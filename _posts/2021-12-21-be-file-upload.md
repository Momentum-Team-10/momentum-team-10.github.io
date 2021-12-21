---
layout: post
title: 🐻 File Upload with Django and DRF 🐻
tags: phase-3 phase-3-be full-text-search deploy file-upload
---

## 🗓️ Today's Topics

- Project Progress
- File Uploads

## 🔖 Resources

### File uploads

- [Django Docs: ImageField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#imagefield)
- [Django Docs: FileField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#filefield)
- [Pillow: Python Imaging Library](https://pillow.readthedocs.io/en/stable/)
  - [`django-imagekit`](https://django-imagekit.readthedocs.io/en/latest/) -> If you want to resize images when they are uploaded, or do any kind of image processing, you will need this. Don't add it unless you know you need it.
- [How to Setup Amazon S3](https://simpleisbetterthancomplex.com/tutorial/2017/08/01/how-to-setup-amazon-s3-in-a-django-project.html)
- [`django-storages`](https://django-storages.readthedocs.io/en/latest/index.html)
- [DRF `FileUploadParser`](https://www.django-rest-framework.org/api-guide/parsers/#fileuploadparser)

#### POST with upload using Insomnia

- Choose binary file attachment from the JSON menu (where you normally put the body of a request)
- Headers (this example assumes an image file in jpeg format, named `profile-photo  .jpg`):

  ```
  Content-Type: image/jpeg
  Content-Disposition: attachment; filename=profile-photo.jpg
  ```

For more information on the values for `Content-Type`:

- [MDN Content-Type Header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Type)
- [MDN MIME types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)

#### CORS for file upload

Assuming you are using `django-cors-headers`, you'll need to add the following to `settings.py`:

```py

from corsheaders.defaults import default_headers

CORS_ALLOW_HEADERS = list(default_headers) + [
    'content-disposition',
]
```

## 📖 Read | 📺 Watch | 🎧 Listen

- 📖 [File Upload with DRF](https://goodcode.io/articles/django-rest-framework-file-upload/)
- 🎧 + 📖 [Success with Static Files](https://www.mattlayman.com/django-riffs/success-static-files/)
- 📖 [What is Amazon S3?](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) -> Skim this -- this is Amazon's documentation and it gets really in-depth.
  - 📺 [Introduction to S3](https://www.youtube.com/watch?v=77lMCiiMilo) -> Also from Amazon
