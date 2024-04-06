git clone https://github.com/HumanSignal/label-studio.git
cd label-studio
pip install poetry
poetry install
poetry run python label_studio/manage.py migrate
poetry run python label_studio/manage.py collectstatic
poetry run python label_studio/manage.py runserver