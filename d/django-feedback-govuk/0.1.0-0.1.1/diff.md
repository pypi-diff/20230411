# Comparing `tmp/django_feedback_govuk-0.1.0.tar.gz` & `tmp/django_feedback_govuk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_feedback_govuk-0.1.0.tar", max compression
+gzip compressed data, was "django_feedback_govuk-0.1.1.tar", max compression
```

## Comparing `django_feedback_govuk-0.1.0.tar` & `django_feedback_govuk-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1091 2023-03-14 11:04:30.618076 django_feedback_govuk-0.1.0/LICENSE
--rw-r--r--   0        0        0     2022 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.0/django_feedback_govuk/__init__.py
--rw-r--r--   0        0        0       95 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.0/django_feedback_govuk/admin.py
--rw-r--r--   0        0        0     1762 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/forms.py
--rw-r--r--   0        0        0     1840 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.0/django_feedback_govuk/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.0/django_feedback_govuk/migrations/__init__.py
--rw-r--r--   0        0        0      920 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.0/django_feedback_govuk/models.py
--rw-r--r--   0        0        0      700 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/notify.py
--rw-r--r--   0        0        0     3357 2023-03-14 16:49:16.438614 django_feedback_govuk-0.1.0/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
--rw-r--r--   0        0        0     2339 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
--rw-r--r--   0        0        0      216 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
--rw-r--r--   0        0        0     1399 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
--rw-r--r--   0        0        0      368 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
--rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
--rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
--rw-r--r--   0        0        0       48 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
--rw-r--r--   0        0        0     1898 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
--rw-r--r--   0        0        0     1737 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
--rw-r--r--   0        0        0        0 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templatetags/__init__.py
--rw-r--r--   0        0        0     1192 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/templatetags/feedback_tags.py
--rw-r--r--   0        0        0      471 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/urls.py
--rw-r--r--   0        0        0     1826 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/django_feedback_govuk/views.py
--rw-r--r--   0        0        0     1789 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.0/setup.py
--rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-14 11:04:30.618076 django_feedback_govuk-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2786 2023-04-11 10:12:43.934435 django_feedback_govuk-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.1/django_feedback_govuk/__init__.py
+-rw-r--r--   0        0        0       95 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.1/django_feedback_govuk/admin.py
+-rw-r--r--   0        0        0     1790 2023-04-11 10:12:43.934435 django_feedback_govuk-0.1.1/django_feedback_govuk/forms.py
+-rw-r--r--   0        0        0     1840 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.1/django_feedback_govuk/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.1/django_feedback_govuk/migrations/__init__.py
+-rw-r--r--   0        0        0      920 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.1/django_feedback_govuk/models.py
+-rw-r--r--   0        0        0      694 2023-04-11 10:12:43.934435 django_feedback_govuk-0.1.1/django_feedback_govuk/notify.py
+-rw-r--r--   0        0        0     2061 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.1/django_feedback_govuk/settings.py
+-rw-r--r--   0        0        0     3357 2023-03-14 16:49:16.438614 django_feedback_govuk-0.1.1/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
+-rw-r--r--   0        0        0     2339 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
+-rw-r--r--   0        0        0      180 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
+-rw-r--r--   0        0        0     1399 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
+-rw-r--r--   0        0        0      351 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
+-rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
+-rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
+-rw-r--r--   0        0        0       48 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
+-rw-r--r--   0        0        0     1898 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
+-rw-r--r--   0        0        0     1737 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
+-rw-r--r--   0        0        0        0 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/templatetags/__init__.py
+-rw-r--r--   0        0        0     1605 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.1/django_feedback_govuk/templatetags/feedback_tags.py
+-rw-r--r--   0        0        0      471 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/urls.py
+-rw-r--r--   0        0        0     1826 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.1/django_feedback_govuk/views.py
+-rw-r--r--   0        0        0     1789 2023-04-11 10:12:43.954435 django_feedback_govuk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4142 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.1/setup.py
+-rw-r--r--   0        0        0     4034 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.1/PKG-INFO
```

### Comparing `django_feedback_govuk-0.1.0/LICENSE` & `django_feedback_govuk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/README.md` & `django_feedback_govuk-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -36,14 +36,30 @@
 GOVUK_NOTIFY_API_KEY="<your-api-key>"
 
 # Django Feedback GovUK
 DJANGO_FEEDBACK_GOVUK = {
     "SERVICE_NAME": "<your-service>",
     "FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
     "FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS": ["email@example.com"],
+    "COPY": {
+        #...add any copy tags to override here
+    }
+}
+
+The copy dict contains string IDs for all user-facing copy, defaulting to the following (override
+just the fields you want to, using the `{{ service_name }}` variable if necessary for _title and _body strings):
+
+```py
+{
+    "SUBMIT_TITLE": "Give feedback on {{ service_name }}",
+    "CONFIRM_TITLE": "Feedback submitted",
+    "CONFIRM_BODY": "Thank you for submitting your feedback.",
+    "FIELD_SATISFACTION_LEGEND": "Overall, how did you feel about the service you received today?",
+    "FIELD_COMMENT_LEGEND": "How could we improve this service?",
+    "FIELD_COMMENT_HINT": "Do not include any personal or financial information, for example your National Insurance or credit card numbers.",
 }
 ```
 
 The email addresses are for every recipient that should get an email when feedback is submitted.
 
 3. Build your own templates
```

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/forms.py` & `django_feedback_govuk-0.1.1/django_feedback_govuk/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from crispy_forms_gds.helper import FormHelper
 from crispy_forms_gds.layout import HTML, Field, Fieldset, Layout, Size, Submit
+from django.conf import settings
 from django.forms import HiddenInput, ModelForm, RadioSelect
 
 from .models import Feedback, SatisfactionOptions
+from .settings import dfg_settings
 
 
 class FeedbackForm(ModelForm):
     class Meta:
         model = Feedback
         fields = ["satisfaction", "comment", "submitter"]
 
@@ -26,22 +28,24 @@
         self.helper.layout = Layout(
             Field("submitter"),
             Fieldset(
                 Field.radios(
                     "satisfaction",
                     template="django_feedback_govuk/widgets/star_rating/star_rating.html",
                 ),
-                legend="Overall, how did you feel about the service you received today?",
+                legend=dfg_settings.COPY_FIELD_SATISFACTION_LEGEND,
                 legend_size=Size.MEDIUM,
             ),
             Fieldset(
                 HTML(
-                    "<p class='govuk-hint'>Do not include any personal or "
-                    "financial information, for example your National "
-                    "Insurance or credit card numbers.</p>"
+                    (
+                        "<p class='govuk-hint'>",
+                        dfg_settings.COPY_FIELD_COMMENT_HINT,
+                        "</p>",
+                    )
                 ),
                 Field("comment"),
-                legend="How could we improve this service?",
+                legend=dfg_settings.COPY_FIELD_COMMENT_LEGEND,
                 legend_size=Size.MEDIUM,
             ),
             Submit("submit", "Send feedback"),
         )
```

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/migrations/0001_initial.py` & `django_feedback_govuk-0.1.1/django_feedback_govuk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/models.py` & `django_feedback_govuk-0.1.1/django_feedback_govuk/models.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/notify.py` & `django_feedback_govuk-0.1.1/django_feedback_govuk/notify.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Dict
 
 from django.conf import settings
 from notifications_python_client.notifications import NotificationsAPIClient
 
+from .settings import dfg_settings
+
 
 def email(personalisation: Dict):
     notification_client = NotificationsAPIClient(
         settings.GOVUK_NOTIFY_API_KEY,
     )
-    email_addresses = settings.DJANGO_FEEDBACK_GOVUK['FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS']
+    email_addresses = dfg_settings.FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS
 
     for email_address in email_addresses:
         message_response = notification_client.send_email_notification(
             email_address=email_address,
-            template_id=settings.DJANGO_FEEDBACK_GOVUK['FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID'],
+            template_id=dfg_settings.FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID,
             personalisation=personalisation,
         )
 
     return message_response
```

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/static/django_feedback_govuk/star-rating.css` & `django_feedback_govuk-0.1.1/django_feedback_govuk/static/django_feedback_govuk/star-rating.css`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html` & `django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html` & `django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html` & `django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html` & `django_feedback_govuk-0.1.1/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/templatetags/feedback_tags.py` & `django_feedback_govuk-0.1.1/django_feedback_govuk/templatetags/feedback_tags.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 from django import template
 from django.conf import settings
+from django.template import Context, Template
 
 from django_feedback_govuk.forms import FeedbackForm
+from django_feedback_govuk.settings import dfg_settings
+
 
 register = template.Library()
 
 
-@register.inclusion_tag("django_feedback_govuk/partials/submit.html", takes_context=True)
+@register.inclusion_tag(
+    "django_feedback_govuk/partials/submit.html", takes_context=True
+)
 def feedback_submit(context):
-    if 'form' in context:
-        form = context['form']
+    if "form" in context:
+        form = context["form"]
     else:
         initial = {}
         initial["submitter"] = context.request.user
         form = FeedbackForm(initial=initial)
 
-    return {
+    new_context = {
         "form": form,
-        "service_name": settings.DJANGO_FEEDBACK_GOVUK["SERVICE_NAME"],
+        "service_name": dfg_settings.SERVICE_NAME,
+        "submit_title": dfg_settings.COPY_SUBMIT_TITLE,
     }
+    return new_context
 
 
-@register.inclusion_tag("django_feedback_govuk/partials/confirm.html")
-def feedback_confirm():
-    return {}
+@register.inclusion_tag(
+    "django_feedback_govuk/partials/confirm.html", takes_context=True
+)
+def feedback_confirm(context):
+    new_context = {
+        "service_name": dfg_settings.SERVICE_NAME,
+        "confirm_title": dfg_settings.COPY_CONFIRM_TITLE,
+        "confirm_body": dfg_settings.COPY_CONFIRM_BODY,
+    }
+    return new_context
 
 
-@register.inclusion_tag("django_feedback_govuk/partials/listing.html", takes_context=True)
+@register.inclusion_tag(
+    "django_feedback_govuk/partials/listing.html", takes_context=True
+)
 def feedback_listing(context):
     return context
 
 
 @register.filter()
 def get_elided_page_range(page):
     return page.paginator.get_elided_page_range(page.number, on_each_side=1, on_ends=1)
```

### Comparing `django_feedback_govuk-0.1.0/django_feedback_govuk/views.py` & `django_feedback_govuk-0.1.1/django_feedback_govuk/views.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.0/pyproject.toml` & `django_feedback_govuk-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-feedback-govuk"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Django app to gather and send internal Government staff feedback"
 authors = ["jafacakes2011 <cameron.lamb@digitial.trade.gov.uk>", "marcelkornblum <marcel.kornblum@digitial.trade.gov.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_feedback_govuk"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `django_feedback_govuk-0.1.0/setup.py` & `django_feedback_govuk-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 ['Django>=3.2,<4.0',
  'crispy-forms-gds>=0.2.4,<0.3.0',
  'django-crispy-forms>=1.9,<2.0',
  'notifications-python-client>=8.0.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'django-feedback-govuk',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A Django app to gather and send internal Government staff feedback',
-    'long_description': '# django-feedback\n\nA Django app to gather and send internal Government staff feedback, e.g. for open beta periods\n\n## Installation\n\n```\npip install django-feedback-govuk\n```\n\n1. Add `django-feedback` to your INSTALLED_APPS settings:\n\n```py\nINSTALLED_APPS = [\n    ...\n    \'crispy_forms\',\n    \'crispy_forms_gds\',\n    \'django_feedback_govuk\',\n]\n```\n\n2. Create a new email template in the GovUk Notify service, making sure to create a ((feedback_url)) field.\n\n> Note that ((feedback_url)) will be a link to the listing view, not an individual piece of feedback.\n\nYou\'ll need an API key and template ID from the gov.uk Notify service.\n\n3. Add the following settings to the file:\n\n```py\n# Crispy forms\nCRISPY_ALLOWED_TEMPLATE_PACKS = ["gds"]\nCRISPY_TEMPLATE_PACK = "gds"\n\n# Gov Notify\nGOVUK_NOTIFY_API_KEY="<your-api-key>"\n\n# Django Feedback GovUK\nDJANGO_FEEDBACK_GOVUK = {\n    "SERVICE_NAME": "<your-service>",\n    "FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",\n    "FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS": ["email@example.com"],\n}\n```\n\nThe email addresses are for every recipient that should get an email when feedback is submitted.\n\n3. Build your own templates\n\nOverride the built-in templates by making new templates in your app under the\n`django_feedback_govuk/templates` path. You\'ll need templates for `submit.html`, `confirm.html`\nand `listing.html`, each of which should load its respective template tag from `feedback_submit`,\n`feedback_confirm` and `feedback_listing`.\n\nFor example:\n\n```py\n{# /your-project/templates/django_feedback_govuk/templates/submit.html #}\n{% extends "base.html" %}\n{% load feedback_tags %}\n{% block content %}\n    {% feedback_submit %}\n{% endblock content %}\n```\n\n> If you\'d like to use the templatetags without causing page loads to new views\n\n4. Add the URLs to your project\n\n```py\nfrom django_feedback_govuk import urls as feedback_urls\n\n\nurlpatterns = [\n    ...\n    path("feedback/", include(feedback_urls)),\n    ...\n]\n```\n\n5. Set up user permissions\n',
+    'long_description': '# django-feedback\n\nA Django app to gather and send internal Government staff feedback, e.g. for open beta periods\n\n## Installation\n\n```\npip install django-feedback-govuk\n```\n\n1. Add `django-feedback` to your INSTALLED_APPS settings:\n\n```py\nINSTALLED_APPS = [\n    ...\n    \'crispy_forms\',\n    \'crispy_forms_gds\',\n    \'django_feedback_govuk\',\n]\n```\n\n2. Create a new email template in the GovUk Notify service, making sure to create a ((feedback_url)) field.\n\n> Note that ((feedback_url)) will be a link to the listing view, not an individual piece of feedback.\n\nYou\'ll need an API key and template ID from the gov.uk Notify service.\n\n3. Add the following settings to the file:\n\n```py\n# Crispy forms\nCRISPY_ALLOWED_TEMPLATE_PACKS = ["gds"]\nCRISPY_TEMPLATE_PACK = "gds"\n\n# Gov Notify\nGOVUK_NOTIFY_API_KEY="<your-api-key>"\n\n# Django Feedback GovUK\nDJANGO_FEEDBACK_GOVUK = {\n    "SERVICE_NAME": "<your-service>",\n    "FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",\n    "FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS": ["email@example.com"],\n    "COPY": {\n        #...add any copy tags to override here\n    }\n}\n\nThe copy dict contains string IDs for all user-facing copy, defaulting to the following (override\njust the fields you want to, using the `{{ service_name }}` variable if necessary for _title and _body strings):\n\n```py\n{\n    "SUBMIT_TITLE": "Give feedback on {{ service_name }}",\n    "CONFIRM_TITLE": "Feedback submitted",\n    "CONFIRM_BODY": "Thank you for submitting your feedback.",\n    "FIELD_SATISFACTION_LEGEND": "Overall, how did you feel about the service you received today?",\n    "FIELD_COMMENT_LEGEND": "How could we improve this service?",\n    "FIELD_COMMENT_HINT": "Do not include any personal or financial information, for example your National Insurance or credit card numbers.",\n}\n```\n\nThe email addresses are for every recipient that should get an email when feedback is submitted.\n\n3. Build your own templates\n\nOverride the built-in templates by making new templates in your app under the\n`django_feedback_govuk/templates` path. You\'ll need templates for `submit.html`, `confirm.html`\nand `listing.html`, each of which should load its respective template tag from `feedback_submit`,\n`feedback_confirm` and `feedback_listing`.\n\nFor example:\n\n```py\n{# /your-project/templates/django_feedback_govuk/templates/submit.html #}\n{% extends "base.html" %}\n{% load feedback_tags %}\n{% block content %}\n    {% feedback_submit %}\n{% endblock content %}\n```\n\n> If you\'d like to use the templatetags without causing page loads to new views\n\n4. Add the URLs to your project\n\n```py\nfrom django_feedback_govuk import urls as feedback_urls\n\n\nurlpatterns = [\n    ...\n    path("feedback/", include(feedback_urls)),\n    ...\n]\n```\n\n5. Set up user permissions\n',
     'author': 'jafacakes2011',
     'author_email': 'cameron.lamb@digitial.trade.gov.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `django_feedback_govuk-0.1.0/PKG-INFO` & `django_feedback_govuk-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feedback-govuk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Django app to gather and send internal Government staff feedback
 License: MIT
 Author: jafacakes2011
 Author-email: cameron.lamb@digitial.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -64,14 +64,30 @@
 GOVUK_NOTIFY_API_KEY="<your-api-key>"
 
 # Django Feedback GovUK
 DJANGO_FEEDBACK_GOVUK = {
     "SERVICE_NAME": "<your-service>",
     "FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
     "FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS": ["email@example.com"],
+    "COPY": {
+        #...add any copy tags to override here
+    }
+}
+
+The copy dict contains string IDs for all user-facing copy, defaulting to the following (override
+just the fields you want to, using the `{{ service_name }}` variable if necessary for _title and _body strings):
+
+```py
+{
+    "SUBMIT_TITLE": "Give feedback on {{ service_name }}",
+    "CONFIRM_TITLE": "Feedback submitted",
+    "CONFIRM_BODY": "Thank you for submitting your feedback.",
+    "FIELD_SATISFACTION_LEGEND": "Overall, how did you feel about the service you received today?",
+    "FIELD_COMMENT_LEGEND": "How could we improve this service?",
+    "FIELD_COMMENT_HINT": "Do not include any personal or financial information, for example your National Insurance or credit card numbers.",
 }
 ```
 
 The email addresses are for every recipient that should get an email when feedback is submitted.
 
 3. Build your own templates
```

