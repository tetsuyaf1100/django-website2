# 静的ファイル配信

* pip install
```
pip install -r requirements.txt
```

* settings.py
```
STATIC_URL = '/assets/'
STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')

STATICFILES_STORAGE = 'whitenoise.storage.CompressedManifestStaticFilesStorage'
```

* collectstatic
```
python manage.py collectstatic
```
