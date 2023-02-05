Do below changes to have application running and uploading files on aws

1. Create a bucket on on S3 which allows public access and enable ACL configuration
2. In settings.py file - change below values for attribute
    AWS_ACCESS_KEY_ID = 'AKIAS5JUC7UPJBPVG3F7'
    AWS_SECRET_ACCESS_KEY = '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'
    AWS_STORAGE_BUCKET_NAME = 'django-s3-demo-1'
3. run 'python manage.py collectstatic' to upload static files on bucket
    it may contains other static files which are related to django admin interface

Tutorial referred - https://youtu.be/ahBG_iLbJPM