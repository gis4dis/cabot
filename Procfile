web:       python manage.py migrate && gunicorn cabot.wsgi -k gevent --log-file - --reload
celery:    celery worker -A cabot --loglevel=INFO --concurrency=16 -Ofair
beat:      celery beat -A cabot --loglevel=INFO
