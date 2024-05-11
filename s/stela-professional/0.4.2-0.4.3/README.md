# Comparing `tmp/stela_professional-0.4.2.tar.gz` & `tmp/stela_professional-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stela_professional-0.4.2.tar", last modified: Sat May 11 14:03:40 2024, max compression
+gzip compressed data, was "stela_professional-0.4.3.tar", last modified: Sat May 11 14:32:30 2024, max compression
```

## Comparing `stela_professional-0.4.2.tar` & `stela_professional-0.4.3.tar`

### file list

```diff
@@ -1,429 +1,430 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:40.264338 stela_professional-0.4.2/
--rw-rw-rw-   0        0        0    35803 2024-01-15 04:02:49.000000 stela_professional-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      133 2024-01-21 05:12:11.000000 stela_professional-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1268 2024-05-11 14:03:40.261342 stela_professional-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-01-15 04:02:49.000000 stela_professional-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.158104 stela_professional-0.4.2/accounts/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.2/accounts/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.2/accounts/admin.py
--rw-rw-rw-   0        0        0      154 2024-01-15 04:02:49.000000 stela_professional-0.4.2/accounts/apps.py
--rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.2/accounts/forms.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.164099 stela_professional-0.4.2/accounts/migrations/
--rw-rw-rw-   0        0        0     4062 2024-01-22 13:09:35.000000 stela_professional-0.4.2/accounts/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-22 13:09:35.000000 stela_professional-0.4.2/accounts/migrations/__init__.py
--rw-rw-rw-   0        0        0     4862 2024-01-16 08:21:22.000000 stela_professional-0.4.2/accounts/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.2/accounts/tests.py
--rw-rw-rw-   0        0        0      370 2024-01-15 04:02:49.000000 stela_professional-0.4.2/accounts/token.py
--rw-rw-rw-   0        0        0     1836 2024-01-15 04:02:49.000000 stela_professional-0.4.2/accounts/urls.py
--rw-rw-rw-   0        0        0    10979 2024-01-15 04:02:49.000000 stela_professional-0.4.2/accounts/views.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.187085 stela_professional-0.4.2/cloud/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.2/cloud/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.2/cloud/admin.py
--rw-rw-rw-   0        0        0      148 2024-01-15 04:02:49.000000 stela_professional-0.4.2/cloud/apps.py
--rw-rw-rw-   0        0        0     3456 2024-01-15 04:02:49.000000 stela_professional-0.4.2/cloud/cart.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.193082 stela_professional-0.4.2/cloud/migrations/
--rw-rw-rw-   0        0        0     5564 2024-01-22 13:10:00.000000 stela_professional-0.4.2/cloud/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-22 13:10:00.000000 stela_professional-0.4.2/cloud/migrations/__init__.py
--rw-rw-rw-   0        0        0     3508 2024-01-15 04:02:49.000000 stela_professional-0.4.2/cloud/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.2/cloud/tests.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.2/cloud/views.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.211071 stela_professional-0.4.2/geolocation/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.2/geolocation/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.2/geolocation/admin.py
--rw-rw-rw-   0        0        0      160 2024-01-15 04:02:49.000000 stela_professional-0.4.2/geolocation/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.218067 stela_professional-0.4.2/geolocation/migrations/
--rw-rw-rw-   0        0        0     6403 2024-01-22 13:10:12.000000 stela_professional-0.4.2/geolocation/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-22 13:10:12.000000 stela_professional-0.4.2/geolocation/migrations/__init__.py
--rw-rw-rw-   0        0        0      582 2024-01-15 04:02:49.000000 stela_professional-0.4.2/geolocation/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.2/geolocation/tests.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.2/geolocation/views.py
--rw-rw-rw-   0        0        0       42 2024-05-11 14:03:40.265339 stela_professional-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1448 2024-05-11 14:03:17.000000 stela_professional-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.300015 stela_professional-0.4.2/stela_control/
--rw-rw-rw-   0        0        0        0 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/__init__.py
--rw-rw-rw-   0        0        0       34 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/admin.py
--rw-rw-rw-   0        0        0      163 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/apps.py
--rw-rw-rw-   0        0        0     7527 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/cart.py
--rw-rw-rw-   0        0        0      164 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/context_processors.py
--rw-rw-rw-   0        0        0      316 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/cron.py
--rw-rw-rw-   0        0        0    86169 2024-05-11 13:24:55.000000 stela_professional-0.4.2/stela_control/forms.py
--rw-rw-rw-   0        0        0      181 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:27.980214 stela_professional-0.4.2/stela_control/locale/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:27.981213 stela_professional-0.4.2/stela_control/locale/es/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.322002 stela_professional-0.4.2/stela_control/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0    55259 2024-02-19 18:04:13.000000 stela_professional-0.4.2/stela_control/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0   332194 2024-02-19 18:03:02.000000 stela_professional-0.4.2/stela_control/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.387962 stela_professional-0.4.2/stela_control/migrations/
--rw-rw-rw-   0        0        0    89195 2024-01-22 13:10:23.000000 stela_professional-0.4.2/stela_control/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     5384 2024-01-22 16:02:46.000000 stela_professional-0.4.2/stela_control/migrations/0002_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6120 2024-01-22 19:38:17.000000 stela_professional-0.4.2/stela_control/migrations/0003_rename_description_company_content_and_more.py
--rw-rw-rw-   0        0        0     5640 2024-01-22 21:09:07.000000 stela_professional-0.4.2/stela_control/migrations/0004_alter_billingrecipt_option_alter_company_address_and_more.py
--rw-rw-rw-   0        0        0     5424 2024-01-22 22:24:05.000000 stela_professional-0.4.2/stela_control/migrations/0005_rename_description_team_content_and_more.py
--rw-rw-rw-   0        0        0     7730 2024-01-31 12:37:18.000000 stela_professional-0.4.2/stela_control/migrations/0006_alter_bankstatement_bank_and_more.py
--rw-rw-rw-   0        0        0     5121 2024-01-31 16:03:17.000000 stela_professional-0.4.2/stela_control/migrations/0007_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5644 2024-02-05 01:43:23.000000 stela_professional-0.4.2/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5171 2024-02-05 07:46:11.000000 stela_professional-0.4.2/stela_control/migrations/0009_content_video_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     4962 2024-02-06 05:55:50.000000 stela_professional-0.4.2/stela_control/migrations/0010_resource_category_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6460 2024-02-06 15:43:12.000000 stela_professional-0.4.2/stela_control/migrations/0011_resource_cover_taxid_pdf_file2_and_more.py
--rw-rw-rw-   0        0        0     5640 2024-02-06 17:11:41.000000 stela_professional-0.4.2/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5323 2024-02-19 17:38:39.000000 stela_professional-0.4.2/stela_control/migrations/0013_content_cover_content_fecade_url_and_more.py
--rw-rw-rw-   0        0        0     5891 2024-02-20 23:29:50.000000 stela_professional-0.4.2/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5039 2024-02-21 15:45:43.000000 stela_professional-0.4.2/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0        0 2024-01-22 13:10:23.000000 stela_professional-0.4.2/stela_control/migrations/__init__.py
--rw-rw-rw-   0        0        0    71703 2024-02-21 15:44:07.000000 stela_professional-0.4.2/stela_control/models.py
--rw-rw-rw-   0        0        0     2943 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/routers.py
--rw-rw-rw-   0        0        0   179145 2024-05-11 13:32:47.000000 stela_professional-0.4.2/stela_control/superfunctions.py
--rw-rw-rw-   0        0        0      410 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/tasks.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:27.983212 stela_professional-0.4.2/stela_control/templates/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.810010 stela_professional-0.4.2/stela_control/templates/stela_control/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.833995 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/
--rw-rw-rw-   0        0        0      497 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/base.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:29.009886 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/registration/
--rw-rw-rw-   0        0        0      227 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/registration/account_activation_email.html
--rw-rw-rw-   0        0        0       21 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/registration/activation_invalid.html
--rw-rw-rw-   0        0        0     1373 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/registration/confirmation_email.html
--rw-rw-rw-   0        0        0     3071 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/registration/register.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:29.281720 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/
--rw-rw-rw-   0        0        0     1364 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/delete_user.html
--rw-rw-rw-   0        0        0     2956 2024-02-06 18:30:10.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/login.html
--rw-rw-rw-   0        0        0     2692 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html
--rw-rw-rw-   0        0        0     2043 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/password_reset_done.html
--rw-rw-rw-   0        0        0      629 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/password_reset_email.html
--rw-rw-rw-   0        0        0     2424 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:29.313700 stela_professional-0.4.2/stela_control/templates/stela_control/analytics/
--rw-rw-rw-   0        0        0      757 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/analytics/analytics.html
--rw-rw-rw-   0        0        0      527 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/analytics/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:29.339684 stela_professional-0.4.2/stela_control/templates/stela_control/api/
--rw-rw-rw-   0        0        0     5932 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/api/main.html
--rw-rw-rw-   0        0        0     2883 2024-01-21 23:59:12.000000 stela_professional-0.4.2/stela_control/templates/stela_control/base.html
--rw-rw-rw-   0        0        0     4402 2024-01-22 14:53:11.000000 stela_professional-0.4.2/stela_control/templates/stela_control/base_content.html
--rw-rw-rw-   0        0        0     6768 2024-01-20 15:13:41.000000 stela_professional-0.4.2/stela_control/templates/stela_control/base_list.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:29.449096 stela_professional-0.4.2/stela_control/templates/stela_control/billing/
--rw-rw-rw-   0        0        0   253007 2024-03-18 11:50:23.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/homebrew.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:29.831707 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/
--rw-rw-rw-   0        0        0     1443 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/bill-data-customer.html
--rw-rw-rw-   0        0        0    30854 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/checkout.html
--rw-rw-rw-   0        0        0      906 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/data-customer.html
--rw-rw-rw-   0        0        0    56802 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/invoice-copy.html
--rw-rw-rw-   0        0        0    56693 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/invoice.html
--rw-rw-rw-   0        0        0     2875 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/order-placed.html
--rw-rw-rw-   0        0        0    48021 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/preview-recipt.html
--rw-rw-rw-   0        0        0     2750 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html
--rw-rw-rw-   0        0        0     3336 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/recipt-detail.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:29.934069 stela_professional-0.4.2/stela_control/templates/stela_control/booking-control/
--rw-rw-rw-   0        0        0     1992 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/booking-control/customer-detail.html
--rw-rw-rw-   0        0        0     4067 2024-01-22 14:58:02.000000 stela_professional-0.4.2/stela_control/templates/stela_control/booking-control/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:29.996286 stela_professional-0.4.2/stela_control/templates/stela_control/chatstela/
--rw-rw-rw-   0        0        0    30842 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/templates/stela_control/chatstela/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.039259 stela_professional-0.4.2/stela_control/templates/stela_control/content/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.100221 stela_professional-0.4.2/stela_control/templates/stela_control/content/comments/
--rw-rw-rw-   0        0        0     2254 2024-01-20 22:35:04.000000 stela_professional-0.4.2/stela_control/templates/stela_control/content/comments/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.157139 stela_professional-0.4.2/stela_control/templates/stela_control/content/docs/
--rw-rw-rw-   0        0        0    10531 2024-02-05 01:03:29.000000 stela_professional-0.4.2/stela_control/templates/stela_control/content/docs/main.html
--rw-rw-rw-   0        0        0     7438 2024-02-06 18:40:47.000000 stela_professional-0.4.2/stela_control/templates/stela_control/content/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.217100 stela_professional-0.4.2/stela_control/templates/stela_control/content/main/
--rw-rw-rw-   0        0        0     1003 2024-02-20 02:42:20.000000 stela_professional-0.4.2/stela_control/templates/stela_control/content/main/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.275064 stela_professional-0.4.2/stela_control/templates/stela_control/content/staff/
--rw-rw-rw-   0        0        0     7608 2024-02-05 04:12:54.000000 stela_professional-0.4.2/stela_control/templates/stela_control/content/staff/index.html
--rw-rw-rw-   0        0        0    26830 2024-02-23 19:08:09.000000 stela_professional-0.4.2/stela_control/templates/stela_control/content/stelastory.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.357014 stela_professional-0.4.2/stela_control/templates/stela_control/developer/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.680815 stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/
--rw-rw-rw-   0        0        0      933 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/modal1.html
--rw-rw-rw-   0        0        0      898 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/modal2.html
--rw-rw-rw-   0        0        0      900 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/modal3.html
--rw-rw-rw-   0        0        0      875 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/modal4.html
--rw-rw-rw-   0        0        0    46793 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/developer/home.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.007198 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.733793 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/accounts/
--rw-rw-rw-   0        0        0      413 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/accounts/password_reset_email.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.831323 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/billing/
--rw-rw-rw-   0        0        0    21938 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html
--rw-rw-rw-   0        0        0    21903 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/billing/invoice.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:30.995222 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/contact/
--rw-rw-rw-   0        0        0    20096 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/contact/message_notification.html
--rw-rw-rw-   0        0        0     8454 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/contact/support_notification.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:31.082169 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/marketing/
--rw-rw-rw-   0        0        0    60992 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:31.130138 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/newsletter/
--rw-rw-rw-   0        0        0    21461 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:31.189101 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/orders/
--rw-rw-rw-   0        0        0    10226 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:31.558238 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/
--rw-rw-rw-   0        0        0    27770 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/billing_payment.html
--rw-rw-rw-   0        0        0     6930 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/charges.html
--rw-rw-rw-   0        0        0    20151 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/payment_notification.html
--rw-rw-rw-   0        0        0    20151 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/sale_notification.html
--rw-rw-rw-   0        0        0     7266 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html
--rw-rw-rw-   0        0        0     7166 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/withdrawals.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:31.610206 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/support/
--rw-rw-rw-   0        0        0    20072 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/support/support_notification.html
--rw-rw-rw-   0        0        0    22345 2024-02-23 19:07:47.000000 stela_professional-0.4.2/stela_control/templates/stela_control/home.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:31.658177 stela_professional-0.4.2/stela_control/templates/stela_control/inbox/
--rw-rw-rw-   0        0        0     2272 2024-01-21 15:59:26.000000 stela_professional-0.4.2/stela_control/templates/stela_control/inbox/index.html
--rw-rw-rw-   0        0        0    11555 2024-02-03 04:29:28.000000 stela_professional-0.4.2/stela_control/templates/stela_control/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.012193 stela_professional-0.4.2/stela_control/templates/stela_control/inventory/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:31.673167 stela_professional-0.4.2/stela_control/templates/stela_control/inventory/products/
--rw-rw-rw-   0        0        0        0 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/inventory/products/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:31.976217 stela_professional-0.4.2/stela_control/templates/stela_control/inventory/resources/
--rw-rw-rw-   0        0        0     2888 2024-01-18 21:03:25.000000 stela_professional-0.4.2/stela_control/templates/stela_control/inventory/resources/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:32.445928 stela_professional-0.4.2/stela_control/templates/stela_control/inventory/services/
--rw-rw-rw-   0        0        0     6806 2024-02-27 00:40:42.000000 stela_professional-0.4.2/stela_control/templates/stela_control/inventory/services/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:32.724757 stela_professional-0.4.2/stela_control/templates/stela_control/jobs/
--rw-rw-rw-   0        0        0     2265 2024-01-22 15:22:45.000000 stela_professional-0.4.2/stela_control/templates/stela_control/jobs/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.170748 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.221717 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutemmerut/
--rw-rw-rw-   0        0        0     1694 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.241704 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutsecondary/
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.311345 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutstela/
--rw-rw-rw-   0        0        0     1381 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutstela/modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.480242 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/alerts/
--rw-rw-rw-   0        0        0      444 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/alerts/budget-alert.html
--rw-rw-rw-   0        0        0      384 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/alerts/budget-success.html
--rw-rw-rw-   0        0        0      404 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/alerts/cancel-recipt.html
--rw-rw-rw-   0        0        0      445 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/alerts/invoice-alert.html
--rw-rw-rw-   0        0        0      380 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/alerts/invoice-success.html
--rw-rw-rw-   0        0        0      471 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/alerts/payeed-recipt.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.504225 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/appstela/
--rw-rw-rw-   0        0        0     1806 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/appstela/modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.021189 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/auth/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.539206 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/auth/pw_reset/
--rw-rw-rw-   0        0        0       45 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/auth/pw_reset/form_errors.html
--rw-rw-rw-   0        0        0      220 2024-01-20 02:10:43.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/auth/pw_reset/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.562191 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/auth/signup/
--rw-rw-rw-   0        0        0      794 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html
--rw-rw-rw-   0        0        0      269 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/auth/signup/success_register.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.639142 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/billing/
--rw-rw-rw-   0        0        0     6947 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/billing/form-billing.html
--rw-rw-rw-   0        0        0    40487 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/billing/recipt-data.html
--rw-rw-rw-   0        0        0     3005 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/blog-feed.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.681117 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/categories/
--rw-rw-rw-   0        0        0      834 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/categories/modal4.html
--rw-rw-rw-   0        0        0      826 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/chatbox.html
--rw-rw-rw-   0        0        0      925 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/chatbox2.html
--rw-rw-rw-   0        0        0      143 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/city_data.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.703108 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/colors/
--rw-rw-rw-   0        0        0      857 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/colors/modal2.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.745631 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/contact/
--rw-rw-rw-   0        0        0     1088 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/contact/form.html
--rw-rw-rw-   0        0        0     1606 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/contact/modal.html
--rw-rw-rw-   0        0        0     1638 2024-01-22 20:05:28.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/dynamic-formset.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.770822 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutfooter/
--rw-rw-rw-   0        0        0     2233 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.836781 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutservices/
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html
--rw-rw-rw-   0        0        0      841 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/form-base.html
--rw-rw-rw-   0        0        0       64 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/form-errors.html
--rw-rw-rw-   0        0        0      924 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/formset-base-services.html
--rw-rw-rw-   0        0        0     1790 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/formset-base.html
--rw-rw-rw-   0        0        0     1569 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/formset.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.029183 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/handlers/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.888747 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/handlers/blog/
--rw-rw-rw-   0        0        0     1469 2024-01-30 20:17:44.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages-v1.html
--rw-rw-rw-   0        0        0      128 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/handlers/blog/empty-blog.html
--rw-rw-rw-   0        0        0      103 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/hashtags.html
--rw-rw-rw-   0        0        0      587 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/instagram-alert.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.938717 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/inventory/
--rw-rw-rw-   0        0        0     1778 2024-02-26 17:25:31.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:33.970696 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/job-application/
--rw-rw-rw-   0        0        0       45 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/job-application/error-form-v1.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:34.088626 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/linkzoneupdates/
--rw-rw-rw-   0        0        0      848 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.036178 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:34.959965 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/
--rw-rw-rw-   0        0        0     1067 2024-02-23 15:58:42.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html
--rw-rw-rw-   0        0        0     1467 2024-02-23 16:29:50.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html
--rw-rw-rw-   0        0        0     1650 2024-02-23 18:05:44.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     2732 2024-02-23 18:06:01.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     2540 2024-02-26 13:05:43.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html
--rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:06.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html
--rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:10.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     2887 2024-02-23 18:06:18.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2593 2024-02-23 18:06:24.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2296 2024-02-23 18:06:30.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1639 2024-02-23 18:06:35.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2587 2024-02-26 13:34:25.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:35.360718 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/
--rw-rw-rw-   0        0        0     1614 2024-02-23 18:04:43.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     3292 2024-02-23 18:04:45.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     3051 2024-02-23 18:04:50.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html
--rw-rw-rw-   0        0        0     1936 2024-02-23 18:04:55.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html
--rw-rw-rw-   0        0        0     2198 2024-02-23 18:05:01.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     2866 2024-02-23 18:05:07.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2737 2024-02-23 18:05:12.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2418 2024-02-23 18:05:17.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1412 2024-02-23 18:07:47.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2803 2024-02-23 18:05:27.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html
--rw-rw-rw-   0        0        0     1297 2024-02-23 15:56:06.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html
--rw-rw-rw-   0        0        0     1778 2024-02-23 16:29:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:35.766596 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/
--rw-rw-rw-   0        0        0     1069 2024-02-23 15:58:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html
--rw-rw-rw-   0        0        0     1464 2024-02-23 16:29:44.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html
--rw-rw-rw-   0        0        0     1962 2024-02-23 18:06:50.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     3022 2024-02-23 18:06:54.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     2878 2024-02-26 13:33:54.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html
--rw-rw-rw-   0        0        0     1740 2024-02-23 18:07:07.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html
--rw-rw-rw-   0        0        0     2080 2024-02-23 18:07:11.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     3148 2024-02-23 18:07:16.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2631 2024-02-23 18:07:22.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2546 2024-04-20 12:39:16.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1929 2024-02-23 18:07:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2616 2024-02-26 14:03:38.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:35.884523 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:35.908508 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/community/
--rw-rw-rw-   0        0        0      818 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/community/formdata.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:35.929493 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/content-pro-media/
--rw-rw-rw-   0        0        0     3209 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.036429 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/content-pro-update/
--rw-rw-rw-   0        0        0       83 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/content-pro-update/content.html
--rw-rw-rw-   0        0        0       84 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/content-pro-update/schedule.html
--rw-rw-rw-   0        0        0      986 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.091395 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ic-update/
--rw-rw-rw-   0        0        0      469 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ic-update/content.html
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.218316 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/
--rw-rw-rw-   0        0        0    25077 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html
--rw-rw-rw-   0        0        0     1667 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html
--rw-rw-rw-   0        0        0     1530 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html
--rw-rw-rw-   0        0        0     1849 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html
--rw-rw-rw-   0        0        0     1774 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html
--rw-rw-rw-   0        0        0     4485 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html
--rw-rw-rw-   0        0        0     5787 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.248298 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/meta-assets/
--rw-rw-rw-   0        0        0        0 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page-alert.html
--rw-rw-rw-   0        0        0      628 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.327249 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/page-analythics/
--rw-rw-rw-   0        0        0     1755 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html
--rw-rw-rw-   0        0        0     1960 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html
--rw-rw-rw-   0        0        0     1428 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.351235 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/smart-boost/
--rw-rw-rw-   0        0        0     2129 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.367225 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/stela-sight/
--rw-rw-rw-   0        0        0      268 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/stela-sight/data.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.412196 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/newcomer/
--rw-rw-rw-   0        0        0     4162 2024-02-06 04:01:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/newcomer/form.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.468164 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/newsletter/
--rw-rw-rw-   0        0        0      216 2024-01-31 02:03:43.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/newsletter/form.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.527125 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/post/
--rw-rw-rw-   0        0        0      846 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/post/list-modal.html
--rw-rw-rw-   0        0        0      850 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/post/main-modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.585090 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/
--rw-rw-rw-   0        0        0     1824 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/catalog-modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.723005 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/
--rw-rw-rw-   0        0        0      933 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/catalog-form.html
--rw-rw-rw-   0        0        0      872 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/category-form.html
--rw-rw-rw-   0        0        0      888 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/color-form.html
--rw-rw-rw-   0        0        0     1024 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/product-form.html
--rw-rw-rw-   0        0        0      855 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/size-form.html
--rw-rw-rw-   0        0        0      115 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/variant-form.html
--rw-rw-rw-   0        0        0      805 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/product-modal.html
--rw-rw-rw-   0        0        0      848 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/size-modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.896444 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/update/
--rw-rw-rw-   0        0        0      234 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/update/catalog-form.html
--rw-rw-rw-   0        0        0      287 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/update/category-form.html
--rw-rw-rw-   0        0        0      230 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/update/color-form.html
--rw-rw-rw-   0        0        0     1008 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/update/product-form.html
--rw-rw-rw-   0        0        0      228 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/update/size-form.html
--rw-rw-rw-   0        0        0      234 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/update/variant-form.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.941417 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/profile/
--rw-rw-rw-   0        0        0     1306 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/profile/dynamic-form.html
--rw-rw-rw-   0        0        0      200 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/profile/single-form.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:36.986389 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/projects/
--rw-rw-rw-   0        0        0     1698 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/projects/modal.html
--rw-rw-rw-   0        0        0      265 2024-01-18 10:44:28.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/remove-complete.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.040355 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/render/
--rw-rw-rw-   0        0        0      143 2024-01-21 14:42:59.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/render/city_data.html
--rw-rw-rw-   0        0        0      604 2024-01-18 10:28:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/single-form.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.062163 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.160281 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/
--rw-rw-rw-   0        0        0     1099 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.233237 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_forms/
--rw-rw-rw-   0        0        0     1099 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.316185 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/forms/
--rw-rw-rw-   0        0        0     1269 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html
--rw-rw-rw-   0        0        0     1097 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.358160 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/update_forms/
--rw-rw-rw-   0        0        0     1156 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html
--rw-rw-rw-   0        0        0     1320 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.386143 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/staff/
--rw-rw-rw-   0        0        0     1947 2024-01-18 10:28:34.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/staff/form.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.508068 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stela_story/
--rw-rw-rw-   0        0        0     3418 2024-02-21 15:38:13.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stela_story/feed-item.html
--rw-rw-rw-   0        0        0     2001 2024-01-18 10:28:39.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.531054 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelafooter/
--rw-rw-rw-   0        0        0     2176 2024-01-18 10:28:39.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelafooter/modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.560036 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelamedia/
--rw-rw-rw-   0        0        0     1695 2024-01-18 10:28:39.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelamedia/modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.585021 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelapath/
--rw-rw-rw-   0        0        0     1337 2024-01-18 10:28:39.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelapath/modal.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.665970 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/
--rw-rw-rw-   0        0        0      663 2024-01-22 15:21:03.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/bank_statements.html
--rw-rw-rw-   0        0        0      675 2024-01-22 15:22:21.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/invoices.html
--rw-rw-rw-   0        0        0      675 2024-01-22 15:22:25.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/retentions.html
--rw-rw-rw-   0        0        0      630 2024-01-22 15:21:30.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/tax-return.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.690956 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/users/
--rw-rw-rw-   0        0        0      254 2024-01-19 18:04:36.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/users/suspend.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.707945 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/youtube/
--rw-rw-rw-   0        0        0      157 2024-01-18 10:28:39.000000 stela_professional-0.4.2/stela_control/templates/stela_control/load-data/youtube/video-preview.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.074157 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:37.764457 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/email-marketing/
--rw-rw-rw-   0        0        0     1543 2024-01-20 22:43:07.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/email-marketing/email_list.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:38.226172 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/
--rw-rw-rw-   0        0        0    10789 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:28.079152 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:38.750341 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/
--rw-rw-rw-   0        0        0    13445 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:38.788652 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/
--rw-rw-rw-   0        0        0    23333 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:38.842620 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/
--rw-rw-rw-   0        0        0    34272 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:38.882593 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:38.915573 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/community/
--rw-rw-rw-   0        0        0    14156 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:39.028504 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/
--rw-rw-rw-   0        0        0    30243 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html
--rw-rw-rw-   0        0        0      248 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/update.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:39.064481 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/
--rw-rw-rw-   0        0        0     3162 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html
--rw-rw-rw-   0        0        0    12633 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html
--rw-rw-rw-   0        0        0    17640 2024-01-22 19:37:49.000000 stela_professional-0.4.2/stela_control/templates/stela_control/newcomer.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:39.127443 stela_professional-0.4.2/stela_control/templates/stela_control/orders/
--rw-rw-rw-   0        0        0     6171 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/orders/list_view.html
--rw-rw-rw-   0        0        0     8860 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/orders/order_update.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:39.375291 stela_professional-0.4.2/stela_control/templates/stela_control/payments/
--rw-rw-rw-   0        0        0    43167 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/payments/homebrew.html
--rw-rw-rw-   0        0        0     2687 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/payments/register-wallet.html
--rw-rw-rw-   0        0        0     4322 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/payments/wallet-list.html
--rw-rw-rw-   0        0        0     2831 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/payments/withdraw.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:39.398277 stela_professional-0.4.2/stela_control/templates/stela_control/prostela/
--rw-rw-rw-   0        0        0      153 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/prostela/chatbox.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:39.431255 stela_professional-0.4.2/stela_control/templates/stela_control/prostela-expert/
--rw-rw-rw-   0        0        0    34014 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/prostela-expert/index.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:39.477227 stela_professional-0.4.2/stela_control/templates/stela_control/reviews/
--rw-rw-rw-   0        0        0     2269 2024-01-20 22:29:12.000000 stela_professional-0.4.2/stela_control/templates/stela_control/reviews/reviews.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:39.591159 stela_professional-0.4.2/stela_control/templates/stela_control/support/
--rw-rw-rw-   0        0        0     6350 2024-01-18 22:16:16.000000 stela_professional-0.4.2/stela_control/templates/stela_control/support/case-detail.html
--rw-rw-rw-   0        0        0     2323 2024-01-18 14:01:39.000000 stela_professional-0.4.2/stela_control/templates/stela_control/support/list.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:40.205376 stela_professional-0.4.2/stela_control/templates/stela_control/users/
--rw-rw-rw-   0        0        0      339 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templates/stela_control/users/generic-user-handler.html
--rw-rw-rw-   0        0        0    11181 2024-01-22 21:22:30.000000 stela_professional-0.4.2/stela_control/templates/stela_control/users/profile.html
--rw-rw-rw-   0        0        0    12343 2024-02-06 16:52:33.000000 stela_professional-0.4.2/stela_control/templates/stela_control/users/users-control.html
--rw-rw-rw-   0        0        0     6472 2024-02-06 15:00:39.000000 stela_professional-0.4.2/stela_control/templates/stela_control/users/users.html
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:40.233358 stela_professional-0.4.2/stela_control/templatetags/
--rw-rw-rw-   0        0        0        0 2024-01-18 10:28:40.000000 stela_professional-0.4.2/stela_control/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1428 2024-04-08 13:35:26.000000 stela_professional-0.4.2/stela_control/templatetags/stelatags.py
--rw-rw-rw-   0        0        0      507 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/tests.py
--rw-rw-rw-   0        0        0     1131 2024-01-18 10:28:32.000000 stela_professional-0.4.2/stela_control/tokenize.py
--rw-rw-rw-   0        0        0     7442 2024-02-20 00:40:50.000000 stela_professional-0.4.2/stela_control/urls.py
--rw-rw-rw-   0        0        0   270343 2024-03-18 11:42:47.000000 stela_professional-0.4.2/stela_control/views.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:03:40.257343 stela_professional-0.4.2/stela_professional.egg-info/
--rw-rw-rw-   0        0        0     1268 2024-05-11 14:03:27.000000 stela_professional-0.4.2/stela_professional.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    20476 2024-05-11 14:03:27.000000 stela_professional-0.4.2/stela_professional.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 14:03:27.000000 stela_professional-0.4.2/stela_professional.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      384 2024-05-11 14:03:27.000000 stela_professional-0.4.2/stela_professional.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2024-05-11 14:03:27.000000 stela_professional-0.4.2/stela_professional.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.598284 stela_professional-0.4.3/
+-rw-rw-rw-   0        0        0    35803 2024-01-15 04:02:49.000000 stela_professional-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0      133 2024-01-21 05:12:11.000000 stela_professional-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1268 2024-05-11 14:32:30.595286 stela_professional-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2024-01-15 04:02:49.000000 stela_professional-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.964334 stela_professional-0.4.3/accounts/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.3/accounts/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.3/accounts/admin.py
+-rw-rw-rw-   0        0        0      154 2024-01-15 04:02:49.000000 stela_professional-0.4.3/accounts/apps.py
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.3/accounts/forms.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.970328 stela_professional-0.4.3/accounts/migrations/
+-rw-rw-rw-   0        0        0     4062 2024-01-22 13:09:35.000000 stela_professional-0.4.3/accounts/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 13:09:35.000000 stela_professional-0.4.3/accounts/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4862 2024-01-16 08:21:22.000000 stela_professional-0.4.3/accounts/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.3/accounts/tests.py
+-rw-rw-rw-   0        0        0      370 2024-01-15 04:02:49.000000 stela_professional-0.4.3/accounts/token.py
+-rw-rw-rw-   0        0        0     1836 2024-01-15 04:02:49.000000 stela_professional-0.4.3/accounts/urls.py
+-rw-rw-rw-   0        0        0    10979 2024-01-15 04:02:49.000000 stela_professional-0.4.3/accounts/views.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.991316 stela_professional-0.4.3/cloud/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.3/cloud/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.3/cloud/admin.py
+-rw-rw-rw-   0        0        0      148 2024-01-15 04:02:49.000000 stela_professional-0.4.3/cloud/apps.py
+-rw-rw-rw-   0        0        0     3456 2024-01-15 04:02:49.000000 stela_professional-0.4.3/cloud/cart.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.998311 stela_professional-0.4.3/cloud/migrations/
+-rw-rw-rw-   0        0        0     5564 2024-01-22 13:10:00.000000 stela_professional-0.4.3/cloud/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 13:10:00.000000 stela_professional-0.4.3/cloud/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3508 2024-01-15 04:02:49.000000 stela_professional-0.4.3/cloud/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.3/cloud/tests.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.3/cloud/views.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.015301 stela_professional-0.4.3/geolocation/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.3/geolocation/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.3/geolocation/admin.py
+-rw-rw-rw-   0        0        0      160 2024-01-15 04:02:49.000000 stela_professional-0.4.3/geolocation/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.023297 stela_professional-0.4.3/geolocation/migrations/
+-rw-rw-rw-   0        0        0     6403 2024-01-22 13:10:12.000000 stela_professional-0.4.3/geolocation/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 13:10:12.000000 stela_professional-0.4.3/geolocation/migrations/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-01-15 04:02:49.000000 stela_professional-0.4.3/geolocation/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.3/geolocation/tests.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.3/geolocation/views.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 14:32:30.599284 stela_professional-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2024-05-11 14:32:15.000000 stela_professional-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.075264 stela_professional-0.4.3/stela_control/
+-rw-rw-rw-   0        0        0        0 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/__init__.py
+-rw-rw-rw-   0        0        0       34 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/admin.py
+-rw-rw-rw-   0        0        0      163 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/apps.py
+-rw-rw-rw-   0        0        0     7527 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/cart.py
+-rw-rw-rw-   0        0        0      164 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/context_processors.py
+-rw-rw-rw-   0        0        0      316 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/cron.py
+-rw-rw-rw-   0        0        0    86169 2024-05-11 13:24:55.000000 stela_professional-0.4.3/stela_control/forms.py
+-rw-rw-rw-   0        0        0      181 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.807772 stela_professional-0.4.3/stela_control/locale/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.807772 stela_professional-0.4.3/stela_control/locale/es/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.083259 stela_professional-0.4.3/stela_control/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    55259 2024-02-19 18:04:13.000000 stela_professional-0.4.3/stela_control/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0   332194 2024-02-19 18:03:02.000000 stela_professional-0.4.3/stela_control/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.186196 stela_professional-0.4.3/stela_control/migrations/
+-rw-rw-rw-   0        0        0    89195 2024-01-22 13:10:23.000000 stela_professional-0.4.3/stela_control/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     5384 2024-01-22 16:02:46.000000 stela_professional-0.4.3/stela_control/migrations/0002_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6120 2024-01-22 19:38:17.000000 stela_professional-0.4.3/stela_control/migrations/0003_rename_description_company_content_and_more.py
+-rw-rw-rw-   0        0        0     5640 2024-01-22 21:09:07.000000 stela_professional-0.4.3/stela_control/migrations/0004_alter_billingrecipt_option_alter_company_address_and_more.py
+-rw-rw-rw-   0        0        0     5424 2024-01-22 22:24:05.000000 stela_professional-0.4.3/stela_control/migrations/0005_rename_description_team_content_and_more.py
+-rw-rw-rw-   0        0        0     7730 2024-01-31 12:37:18.000000 stela_professional-0.4.3/stela_control/migrations/0006_alter_bankstatement_bank_and_more.py
+-rw-rw-rw-   0        0        0     5121 2024-01-31 16:03:17.000000 stela_professional-0.4.3/stela_control/migrations/0007_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5644 2024-02-05 01:43:23.000000 stela_professional-0.4.3/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5171 2024-02-05 07:46:11.000000 stela_professional-0.4.3/stela_control/migrations/0009_content_video_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     4962 2024-02-06 05:55:50.000000 stela_professional-0.4.3/stela_control/migrations/0010_resource_category_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6460 2024-02-06 15:43:12.000000 stela_professional-0.4.3/stela_control/migrations/0011_resource_cover_taxid_pdf_file2_and_more.py
+-rw-rw-rw-   0        0        0     5640 2024-02-06 17:11:41.000000 stela_professional-0.4.3/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5323 2024-02-19 17:38:39.000000 stela_professional-0.4.3/stela_control/migrations/0013_content_cover_content_fecade_url_and_more.py
+-rw-rw-rw-   0        0        0     5891 2024-02-20 23:29:50.000000 stela_professional-0.4.3/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5039 2024-02-21 15:45:43.000000 stela_professional-0.4.3/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 13:10:23.000000 stela_professional-0.4.3/stela_control/migrations/__init__.py
+-rw-rw-rw-   0        0        0    71703 2024-02-21 15:44:07.000000 stela_professional-0.4.3/stela_control/models.py
+-rw-rw-rw-   0        0        0     2943 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/routers.py
+-rw-rw-rw-   0        0        0   179145 2024-05-11 13:32:47.000000 stela_professional-0.4.3/stela_control/superfunctions.py
+-rw-rw-rw-   0        0        0      410 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/tasks.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.810769 stela_professional-0.4.3/stela_control/templates/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.312118 stela_professional-0.4.3/stela_control/templates/stela_control/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.333105 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/
+-rw-rw-rw-   0        0        0      497 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/base.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.382075 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/registration/
+-rw-rw-rw-   0        0        0      227 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/registration/account_activation_email.html
+-rw-rw-rw-   0        0        0       21 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/registration/activation_invalid.html
+-rw-rw-rw-   0        0        0     1373 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/registration/confirmation_email.html
+-rw-rw-rw-   0        0        0     3071 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/registration/register.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.547973 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/
+-rw-rw-rw-   0        0        0     1364 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/delete_user.html
+-rw-rw-rw-   0        0        0     2956 2024-02-06 18:30:10.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/login.html
+-rw-rw-rw-   0        0        0     2692 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html
+-rw-rw-rw-   0        0        0     2043 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/password_reset_done.html
+-rw-rw-rw-   0        0        0      629 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/password_reset_email.html
+-rw-rw-rw-   0        0        0     2424 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.565964 stela_professional-0.4.3/stela_control/templates/stela_control/analytics/
+-rw-rw-rw-   0        0        0      757 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/analytics/analytics.html
+-rw-rw-rw-   0        0        0      527 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/analytics/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.579954 stela_professional-0.4.3/stela_control/templates/stela_control/api/
+-rw-rw-rw-   0        0        0     5932 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/api/main.html
+-rw-rw-rw-   0        0        0     2883 2024-01-21 23:59:12.000000 stela_professional-0.4.3/stela_control/templates/stela_control/base.html
+-rw-rw-rw-   0        0        0     4402 2024-01-22 14:53:11.000000 stela_professional-0.4.3/stela_control/templates/stela_control/base_content.html
+-rw-rw-rw-   0        0        0     6768 2024-01-20 15:13:41.000000 stela_professional-0.4.3/stela_control/templates/stela_control/base_list.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.594514 stela_professional-0.4.3/stela_control/templates/stela_control/billing/
+-rw-rw-rw-   0        0        0   253007 2024-03-18 11:50:23.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/homebrew.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.904786 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/
+-rw-rw-rw-   0        0        0     1443 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/bill-data-customer.html
+-rw-rw-rw-   0        0        0    30854 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/checkout.html
+-rw-rw-rw-   0        0        0      906 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/data-customer.html
+-rw-rw-rw-   0        0        0    56802 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/invoice-copy.html
+-rw-rw-rw-   0        0        0    56693 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/invoice.html
+-rw-rw-rw-   0        0        0     2875 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/order-placed.html
+-rw-rw-rw-   0        0        0    48021 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/preview-recipt.html
+-rw-rw-rw-   0        0        0     2750 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html
+-rw-rw-rw-   0        0        0     3336 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/recipt-detail.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.933769 stela_professional-0.4.3/stela_control/templates/stela_control/booking-control/
+-rw-rw-rw-   0        0        0     1992 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/booking-control/customer-detail.html
+-rw-rw-rw-   0        0        0     4067 2024-01-22 14:58:02.000000 stela_professional-0.4.3/stela_control/templates/stela_control/booking-control/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:25.950758 stela_professional-0.4.3/stela_control/templates/stela_control/chatstela/
+-rw-rw-rw-   0        0        0    30842 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/templates/stela_control/chatstela/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.000727 stela_professional-0.4.3/stela_control/templates/stela_control/content/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.018717 stela_professional-0.4.3/stela_control/templates/stela_control/content/comments/
+-rw-rw-rw-   0        0        0     2390 2024-05-11 14:32:00.000000 stela_professional-0.4.3/stela_control/templates/stela_control/content/comments/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.031708 stela_professional-0.4.3/stela_control/templates/stela_control/content/docs/
+-rw-rw-rw-   0        0        0    10531 2024-02-05 01:03:29.000000 stela_professional-0.4.3/stela_control/templates/stela_control/content/docs/main.html
+-rw-rw-rw-   0        0        0     7438 2024-02-06 18:40:47.000000 stela_professional-0.4.3/stela_control/templates/stela_control/content/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.047698 stela_professional-0.4.3/stela_control/templates/stela_control/content/main/
+-rw-rw-rw-   0        0        0     1003 2024-02-20 02:42:20.000000 stela_professional-0.4.3/stela_control/templates/stela_control/content/main/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.062689 stela_professional-0.4.3/stela_control/templates/stela_control/content/staff/
+-rw-rw-rw-   0        0        0     7608 2024-02-05 04:12:54.000000 stela_professional-0.4.3/stela_control/templates/stela_control/content/staff/index.html
+-rw-rw-rw-   0        0        0    26830 2024-02-23 19:08:09.000000 stela_professional-0.4.3/stela_control/templates/stela_control/content/stelastory.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.078680 stela_professional-0.4.3/stela_control/templates/stela_control/developer/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.163627 stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/
+-rw-rw-rw-   0        0        0      933 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/modal1.html
+-rw-rw-rw-   0        0        0      898 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/modal2.html
+-rw-rw-rw-   0        0        0      900 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/modal3.html
+-rw-rw-rw-   0        0        0      875 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/modal4.html
+-rw-rw-rw-   0        0        0    46793 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/developer/home.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.835414 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.179617 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/accounts/
+-rw-rw-rw-   0        0        0      413 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/accounts/password_reset_email.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.209598 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/billing/
+-rw-rw-rw-   0        0        0    21938 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html
+-rw-rw-rw-   0        0        0    21903 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/billing/invoice.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.244576 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/contact/
+-rw-rw-rw-   0        0        0    20096 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/contact/message_notification.html
+-rw-rw-rw-   0        0        0     8454 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/contact/support_notification.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.258569 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/marketing/
+-rw-rw-rw-   0        0        0    60992 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.274558 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/newsletter/
+-rw-rw-rw-   0        0        0    21461 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.283553 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/orders/
+-rw-rw-rw-   0        0        0    10226 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.384491 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/
+-rw-rw-rw-   0        0        0    27770 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/billing_payment.html
+-rw-rw-rw-   0        0        0     6930 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/charges.html
+-rw-rw-rw-   0        0        0    20151 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/payment_notification.html
+-rw-rw-rw-   0        0        0    20151 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/sale_notification.html
+-rw-rw-rw-   0        0        0     7266 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html
+-rw-rw-rw-   0        0        0     7166 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/withdrawals.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.403479 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/support/
+-rw-rw-rw-   0        0        0    20072 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/support/support_notification.html
+-rw-rw-rw-   0        0        0    22345 2024-02-23 19:07:47.000000 stela_professional-0.4.3/stela_control/templates/stela_control/home.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.420468 stela_professional-0.4.3/stela_control/templates/stela_control/inbox/
+-rw-rw-rw-   0        0        0     2272 2024-01-21 15:59:26.000000 stela_professional-0.4.3/stela_control/templates/stela_control/inbox/index.html
+-rw-rw-rw-   0        0        0    11555 2024-02-03 04:29:28.000000 stela_professional-0.4.3/stela_control/templates/stela_control/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.840410 stela_professional-0.4.3/stela_control/templates/stela_control/inventory/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.438458 stela_professional-0.4.3/stela_control/templates/stela_control/inventory/products/
+-rw-rw-rw-   0        0        0        0 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/inventory/products/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.441456 stela_professional-0.4.3/stela_control/templates/stela_control/inventory/resources/
+-rw-rw-rw-   0        0        0     2888 2024-01-18 21:03:25.000000 stela_professional-0.4.3/stela_control/templates/stela_control/inventory/resources/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:26.905765 stela_professional-0.4.3/stela_control/templates/stela_control/inventory/services/
+-rw-rw-rw-   0        0        0     6806 2024-02-27 00:40:42.000000 stela_professional-0.4.3/stela_control/templates/stela_control/inventory/services/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.155611 stela_professional-0.4.3/stela_control/templates/stela_control/jobs/
+-rw-rw-rw-   0        0        0     2265 2024-01-22 15:22:45.000000 stela_professional-0.4.3/stela_control/templates/stela_control/jobs/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.346493 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.359485 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutemmerut/
+-rw-rw-rw-   0        0        0     1694 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.374476 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutsecondary/
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.384470 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutstela/
+-rw-rw-rw-   0        0        0     1381 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutstela/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.460424 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/alerts/
+-rw-rw-rw-   0        0        0      444 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/alerts/budget-alert.html
+-rw-rw-rw-   0        0        0      384 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/alerts/budget-success.html
+-rw-rw-rw-   0        0        0      404 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/alerts/cancel-recipt.html
+-rw-rw-rw-   0        0        0      445 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/alerts/invoice-alert.html
+-rw-rw-rw-   0        0        0      380 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/alerts/invoice-success.html
+-rw-rw-rw-   0        0        0      471 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/alerts/payeed-recipt.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.476414 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/appstela/
+-rw-rw-rw-   0        0        0     1806 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/appstela/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.850403 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/auth/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.498400 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/auth/pw_reset/
+-rw-rw-rw-   0        0        0       45 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/auth/pw_reset/form_errors.html
+-rw-rw-rw-   0        0        0      220 2024-01-20 02:10:43.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/auth/pw_reset/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.515389 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/auth/signup/
+-rw-rw-rw-   0        0        0      794 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html
+-rw-rw-rw-   0        0        0      269 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/auth/signup/success_register.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.536377 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/billing/
+-rw-rw-rw-   0        0        0     6947 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/billing/form-billing.html
+-rw-rw-rw-   0        0        0    40487 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/billing/recipt-data.html
+-rw-rw-rw-   0        0        0     3005 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/blog-feed.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.576352 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/categories/
+-rw-rw-rw-   0        0        0      834 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/categories/modal4.html
+-rw-rw-rw-   0        0        0      826 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/chatbox.html
+-rw-rw-rw-   0        0        0      925 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/chatbox2.html
+-rw-rw-rw-   0        0        0      143 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/city_data.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.592343 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/colors/
+-rw-rw-rw-   0        0        0      857 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/colors/modal2.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.625322 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/contact/
+-rw-rw-rw-   0        0        0     1088 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/contact/form.html
+-rw-rw-rw-   0        0        0     1606 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/contact/modal.html
+-rw-rw-rw-   0        0        0     1638 2024-01-22 20:05:28.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/dynamic-formset.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.636315 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutfooter/
+-rw-rw-rw-   0        0        0     2233 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.708270 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutservices/
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html
+-rw-rw-rw-   0        0        0      841 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/form-base.html
+-rw-rw-rw-   0        0        0       64 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/form-errors.html
+-rw-rw-rw-   0        0        0       15 2024-05-11 14:18:59.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/form.html
+-rw-rw-rw-   0        0        0      924 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/formset-base-services.html
+-rw-rw-rw-   0        0        0     1790 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/formset-base.html
+-rw-rw-rw-   0        0        0     1569 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/formset.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.861397 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/handlers/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.731257 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/handlers/blog/
+-rw-rw-rw-   0        0        0     1469 2024-01-30 20:17:44.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages-v1.html
+-rw-rw-rw-   0        0        0      128 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/handlers/blog/empty-blog.html
+-rw-rw-rw-   0        0        0      103 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/hashtags.html
+-rw-rw-rw-   0        0        0      587 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/instagram-alert.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.748246 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/inventory/
+-rw-rw-rw-   0        0        0     1778 2024-02-26 17:25:31.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.765236 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/job-application/
+-rw-rw-rw-   0        0        0       45 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/job-application/error-form-v1.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.770232 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/linkzoneupdates/
+-rw-rw-rw-   0        0        0      848 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.870391 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:27.992905 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/
+-rw-rw-rw-   0        0        0     1067 2024-02-23 15:58:42.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html
+-rw-rw-rw-   0        0        0     1467 2024-02-23 16:29:50.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html
+-rw-rw-rw-   0        0        0     1650 2024-02-23 18:05:44.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     2732 2024-02-23 18:06:01.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     2540 2024-02-26 13:05:43.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:06.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:10.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     2887 2024-02-23 18:06:18.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2593 2024-02-23 18:06:24.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2296 2024-02-23 18:06:30.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1639 2024-02-23 18:06:35.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2587 2024-02-26 13:34:25.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.198777 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/
+-rw-rw-rw-   0        0        0     1614 2024-02-23 18:04:43.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     3292 2024-02-23 18:04:45.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     3051 2024-02-23 18:04:50.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1936 2024-02-23 18:04:55.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     2198 2024-02-23 18:05:01.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     2866 2024-02-23 18:05:07.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2737 2024-02-23 18:05:12.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2418 2024-02-23 18:05:17.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1412 2024-02-23 18:07:47.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2803 2024-02-23 18:05:27.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html
+-rw-rw-rw-   0        0        0     1297 2024-02-23 15:56:06.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html
+-rw-rw-rw-   0        0        0     1778 2024-02-23 16:29:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.388662 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/
+-rw-rw-rw-   0        0        0     1069 2024-02-23 15:58:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html
+-rw-rw-rw-   0        0        0     1464 2024-02-23 16:29:44.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html
+-rw-rw-rw-   0        0        0     1962 2024-02-23 18:06:50.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     3022 2024-02-23 18:06:54.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     2878 2024-02-26 13:33:54.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1740 2024-02-23 18:07:07.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     2080 2024-02-23 18:07:11.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     3148 2024-02-23 18:07:16.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2631 2024-02-23 18:07:22.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2546 2024-04-20 12:39:16.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1929 2024-02-23 18:07:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2616 2024-02-26 14:03:38.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.473608 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.488599 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/community/
+-rw-rw-rw-   0        0        0      818 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/community/formdata.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.494595 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/content-pro-media/
+-rw-rw-rw-   0        0        0     3209 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.516581 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/content-pro-update/
+-rw-rw-rw-   0        0        0       83 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/content-pro-update/content.html
+-rw-rw-rw-   0        0        0       84 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/content-pro-update/schedule.html
+-rw-rw-rw-   0        0        0      986 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.533572 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ic-update/
+-rw-rw-rw-   0        0        0      469 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ic-update/content.html
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.596531 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/
+-rw-rw-rw-   0        0        0    25077 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html
+-rw-rw-rw-   0        0        0     1667 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html
+-rw-rw-rw-   0        0        0     1530 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html
+-rw-rw-rw-   0        0        0     1849 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html
+-rw-rw-rw-   0        0        0     1774 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html
+-rw-rw-rw-   0        0        0     4485 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html
+-rw-rw-rw-   0        0        0     5787 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.611524 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/meta-assets/
+-rw-rw-rw-   0        0        0        0 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page-alert.html
+-rw-rw-rw-   0        0        0      628 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.677482 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/page-analythics/
+-rw-rw-rw-   0        0        0     1755 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html
+-rw-rw-rw-   0        0        0     1960 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html
+-rw-rw-rw-   0        0        0     1428 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.692473 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/smart-boost/
+-rw-rw-rw-   0        0        0     2129 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.759432 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/stela-sight/
+-rw-rw-rw-   0        0        0      268 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/stela-sight/data.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.766429 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/newcomer/
+-rw-rw-rw-   0        0        0     4162 2024-02-06 04:01:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/newcomer/form.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.779420 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/newsletter/
+-rw-rw-rw-   0        0        0      216 2024-01-31 02:03:43.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/newsletter/form.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.800407 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/post/
+-rw-rw-rw-   0        0        0      846 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/post/list-modal.html
+-rw-rw-rw-   0        0        0      850 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/post/main-modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.837385 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/
+-rw-rw-rw-   0        0        0     1824 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/catalog-modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:28.929190 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/
+-rw-rw-rw-   0        0        0      933 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/catalog-form.html
+-rw-rw-rw-   0        0        0      872 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/category-form.html
+-rw-rw-rw-   0        0        0      888 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/color-form.html
+-rw-rw-rw-   0        0        0     1024 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/product-form.html
+-rw-rw-rw-   0        0        0      855 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/size-form.html
+-rw-rw-rw-   0        0        0      115 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/variant-form.html
+-rw-rw-rw-   0        0        0      805 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/product-modal.html
+-rw-rw-rw-   0        0        0      848 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/size-modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.017135 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/update/
+-rw-rw-rw-   0        0        0      234 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/update/catalog-form.html
+-rw-rw-rw-   0        0        0      287 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/update/category-form.html
+-rw-rw-rw-   0        0        0      230 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/update/color-form.html
+-rw-rw-rw-   0        0        0     1008 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/update/product-form.html
+-rw-rw-rw-   0        0        0      228 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/update/size-form.html
+-rw-rw-rw-   0        0        0      234 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/update/variant-form.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.046117 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/profile/
+-rw-rw-rw-   0        0        0     1306 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/profile/dynamic-form.html
+-rw-rw-rw-   0        0        0      200 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/profile/single-form.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.058112 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/projects/
+-rw-rw-rw-   0        0        0     1698 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/projects/modal.html
+-rw-rw-rw-   0        0        0      265 2024-01-18 10:44:28.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/remove-complete.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.072102 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/render/
+-rw-rw-rw-   0        0        0      143 2024-01-21 14:42:59.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/render/city_data.html
+-rw-rw-rw-   0        0        0      604 2024-01-18 10:28:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/single-form.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.896375 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.099084 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/
+-rw-rw-rw-   0        0        0     1099 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.132065 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_forms/
+-rw-rw-rw-   0        0        0     1099 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.183033 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/forms/
+-rw-rw-rw-   0        0        0     1269 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html
+-rw-rw-rw-   0        0        0     1097 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.218566 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/update_forms/
+-rw-rw-rw-   0        0        0     1156 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1320 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.236553 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/staff/
+-rw-rw-rw-   0        0        0     1947 2024-01-18 10:28:34.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/staff/form.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.267534 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stela_story/
+-rw-rw-rw-   0        0        0     3418 2024-02-21 15:38:13.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stela_story/feed-item.html
+-rw-rw-rw-   0        0        0     2001 2024-01-18 10:28:39.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.281525 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelafooter/
+-rw-rw-rw-   0        0        0     2176 2024-01-18 10:28:39.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelafooter/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.319502 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelamedia/
+-rw-rw-rw-   0        0        0     1695 2024-01-18 10:28:39.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelamedia/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.331494 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelapath/
+-rw-rw-rw-   0        0        0     1337 2024-01-18 10:28:39.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelapath/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.393457 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/
+-rw-rw-rw-   0        0        0      663 2024-01-22 15:21:03.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/bank_statements.html
+-rw-rw-rw-   0        0        0      675 2024-01-22 15:22:21.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/invoices.html
+-rw-rw-rw-   0        0        0      675 2024-01-22 15:22:25.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/retentions.html
+-rw-rw-rw-   0        0        0      630 2024-01-22 15:21:30.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/tax-return.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.406451 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/users/
+-rw-rw-rw-   0        0        0      254 2024-01-19 18:04:36.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/users/suspend.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.420440 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/youtube/
+-rw-rw-rw-   0        0        0      157 2024-01-18 10:28:39.000000 stela_professional-0.4.3/stela_control/templates/stela_control/load-data/youtube/video-preview.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.906368 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.428435 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/email-marketing/
+-rw-rw-rw-   0        0        0     1543 2024-01-20 22:43:07.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/email-marketing/email_list.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.445425 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/
+-rw-rw-rw-   0        0        0    10789 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:24.910366 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.868147 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/
+-rw-rw-rw-   0        0        0    13445 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.897127 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/
+-rw-rw-rw-   0        0        0    23333 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.919115 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/
+-rw-rw-rw-   0        0        0    34272 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.959091 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:29.974081 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/community/
+-rw-rw-rw-   0        0        0    14156 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.048035 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/
+-rw-rw-rw-   0        0        0    30243 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html
+-rw-rw-rw-   0        0        0      248 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/update.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.060028 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/
+-rw-rw-rw-   0        0        0     3162 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html
+-rw-rw-rw-   0        0        0    12633 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html
+-rw-rw-rw-   0        0        0    17640 2024-01-22 19:37:49.000000 stela_professional-0.4.3/stela_control/templates/stela_control/newcomer.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.093008 stela_professional-0.4.3/stela_control/templates/stela_control/orders/
+-rw-rw-rw-   0        0        0     6171 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/orders/list_view.html
+-rw-rw-rw-   0        0        0     8860 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/orders/order_update.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.178954 stela_professional-0.4.3/stela_control/templates/stela_control/payments/
+-rw-rw-rw-   0        0        0    43167 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/payments/homebrew.html
+-rw-rw-rw-   0        0        0     2687 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/payments/register-wallet.html
+-rw-rw-rw-   0        0        0     4322 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/payments/wallet-list.html
+-rw-rw-rw-   0        0        0     2831 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/payments/withdraw.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.192946 stela_professional-0.4.3/stela_control/templates/stela_control/prostela/
+-rw-rw-rw-   0        0        0      153 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/prostela/chatbox.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.206937 stela_professional-0.4.3/stela_control/templates/stela_control/prostela-expert/
+-rw-rw-rw-   0        0        0    34014 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/prostela-expert/index.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.272896 stela_professional-0.4.3/stela_control/templates/stela_control/reviews/
+-rw-rw-rw-   0        0        0     2269 2024-01-20 22:29:12.000000 stela_professional-0.4.3/stela_control/templates/stela_control/reviews/reviews.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.299880 stela_professional-0.4.3/stela_control/templates/stela_control/support/
+-rw-rw-rw-   0        0        0     6350 2024-01-18 22:16:16.000000 stela_professional-0.4.3/stela_control/templates/stela_control/support/case-detail.html
+-rw-rw-rw-   0        0        0     2323 2024-01-18 14:01:39.000000 stela_professional-0.4.3/stela_control/templates/stela_control/support/list.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.554313 stela_professional-0.4.3/stela_control/templates/stela_control/users/
+-rw-rw-rw-   0        0        0      339 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templates/stela_control/users/generic-user-handler.html
+-rw-rw-rw-   0        0        0    11181 2024-01-22 21:22:30.000000 stela_professional-0.4.3/stela_control/templates/stela_control/users/profile.html
+-rw-rw-rw-   0        0        0    12343 2024-02-06 16:52:33.000000 stela_professional-0.4.3/stela_control/templates/stela_control/users/users-control.html
+-rw-rw-rw-   0        0        0     6472 2024-02-06 15:00:39.000000 stela_professional-0.4.3/stela_control/templates/stela_control/users/users.html
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.569301 stela_professional-0.4.3/stela_control/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-01-18 10:28:40.000000 stela_professional-0.4.3/stela_control/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1428 2024-04-08 13:35:26.000000 stela_professional-0.4.3/stela_control/templatetags/stelatags.py
+-rw-rw-rw-   0        0        0      507 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/tests.py
+-rw-rw-rw-   0        0        0     1131 2024-01-18 10:28:32.000000 stela_professional-0.4.3/stela_control/tokenize.py
+-rw-rw-rw-   0        0        0     7442 2024-02-20 00:40:50.000000 stela_professional-0.4.3/stela_control/urls.py
+-rw-rw-rw-   0        0        0   270343 2024-03-18 11:42:47.000000 stela_professional-0.4.3/stela_control/views.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:32:30.592288 stela_professional-0.4.3/stela_professional.egg-info/
+-rw-rw-rw-   0        0        0     1268 2024-05-11 14:32:24.000000 stela_professional-0.4.3/stela_professional.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    20534 2024-05-11 14:32:24.000000 stela_professional-0.4.3/stela_professional.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 14:32:24.000000 stela_professional-0.4.3/stela_professional.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      384 2024-05-11 14:32:24.000000 stela_professional-0.4.3/stela_professional.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2024-05-11 14:32:24.000000 stela_professional-0.4.3/stela_professional.egg-info/top_level.txt
```

### Comparing `stela_professional-0.4.2/LICENSE` & `stela_professional-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/PKG-INFO` & `stela_professional-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stela_professional
-Version: 0.4.2
+Version: 0.4.3
 Summary: All apps in one for business.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stela_professional-0.4.2/accounts/migrations/0001_initial.py` & `stela_professional-0.4.3/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/accounts/models.py` & `stela_professional-0.4.3/accounts/models.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/accounts/urls.py` & `stela_professional-0.4.3/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/accounts/views.py` & `stela_professional-0.4.3/accounts/views.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/cloud/cart.py` & `stela_professional-0.4.3/cloud/cart.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/cloud/migrations/0001_initial.py` & `stela_professional-0.4.3/cloud/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/cloud/models.py` & `stela_professional-0.4.3/cloud/models.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/geolocation/migrations/0001_initial.py` & `stela_professional-0.4.3/geolocation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/geolocation/models.py` & `stela_professional-0.4.3/geolocation/models.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/setup.py` & `stela_professional-0.4.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 excluded_packages = [
     'core', 'core.*', 
     'linkzone', 'linkzone.*', 
 ]
 setup(
     name='stela_professional',
-    version='0.4.2',
+    version='0.4.3',
     packages=find_packages(exclude=excluded_packages),
     include_package_data=True,
     license='MIT',
     description='All apps in one for business.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

### Comparing `stela_professional-0.4.2/stela_control/cart.py` & `stela_professional-0.4.3/stela_control/cart.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/forms.py` & `stela_professional-0.4.3/stela_control/forms.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/locale/es/LC_MESSAGES/django.mo` & `stela_professional-0.4.3/stela_control/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/locale/es/LC_MESSAGES/django.po` & `stela_professional-0.4.3/stela_control/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0001_initial.py` & `stela_professional-0.4.3/stela_control/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0002_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0002_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0003_rename_description_company_content_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0003_rename_description_company_content_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0004_alter_billingrecipt_option_alter_company_address_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0004_alter_billingrecipt_option_alter_company_address_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0005_rename_description_team_content_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0005_rename_description_team_content_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0006_alter_bankstatement_bank_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0006_alter_bankstatement_bank_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0007_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0007_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0009_content_video_alter_billingrecipt_option_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0009_content_video_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0010_resource_category_alter_billingrecipt_option_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0010_resource_category_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0011_resource_cover_taxid_pdf_file2_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0011_resource_cover_taxid_pdf_file2_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0013_content_cover_content_fecade_url_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0013_content_cover_content_fecade_url_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.3/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/models.py` & `stela_professional-0.4.3/stela_control/models.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/routers.py` & `stela_professional-0.4.3/stela_control/routers.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/superfunctions.py` & `stela_professional-0.4.3/stela_control/superfunctions.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/accounts/registration/confirmation_email.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/accounts/registration/confirmation_email.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/accounts/registration/register.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/accounts/registration/register.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/delete_user.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/delete_user.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/login.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/login.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/password_reset_done.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/password_reset_email.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/accounts/user/password_reset_form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/accounts/user/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/analytics/analytics.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/analytics/analytics.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/analytics/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/analytics/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/api/main.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/api/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/base.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/base.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/base_content.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/base_content.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/base_list.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/base_list.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/homebrew.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/homebrew.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/bill-data-customer.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/bill-data-customer.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/checkout.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/checkout.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/data-customer.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/data-customer.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/invoice-copy.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/invoice-copy.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/invoice.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/invoice.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/order-placed.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/order-placed.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/preview-recipt.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/preview-recipt.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/billing/sections/recipt-detail.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/billing/sections/recipt-detail.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/booking-control/customer-detail.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/booking-control/customer-detail.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/booking-control/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/booking-control/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/chatstela/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/chatstela/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/content/comments/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/content/comments/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     <h1 class="oxanium mx-4 text-dark pt-3">{% trans "Comments" %} <i class="fa-solid fa-comment"></i></h1>
 {% endblock  %}
 {% block side_title %}
     <h3 class="oxanium mx-4 d-flex justify-content-end"><b>STELA {% trans "CONTROL DYNAMIC" %} | {% trans "Content" %}</b></h3>
 {% endblock  %}
 {% block topButtons %}
     <div class="col-lg-2 col-md-6">
-        <button type="submit" class="btn btn-danger btn-danger px-3 mb-3 mx-2 delete-product hide" id="delete_btn">{% trans "Remove" %} <i class="fas fa-trash"></i></button>
+        <button type="submit" data-bs-toggle="modal" data-bs-target="#removeObj" onclick="removeObjListRequest('Comments')" class="btn btn-sm btn-danger btn-block delete-product hide mb-3" id="delete_btn"><span class="oxanium fs-6">Eliminar</span> <i class="fas fa-trash fs-6" aria-hidden="true"></i></button>
     </div>
 {% endblock  %}
 {% block listTitle %}
     <h3 class="text-center fw-bold oxanium fs-4 my-2">{% trans "Comments List" %}</h3>
 {% endblock  %}
 {% block thead %}
     <th style="width: 5%;">Id</th>
```

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/content/docs/main.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/content/docs/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/content/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/content/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/content/main/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/content/main/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/content/staff/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/content/staff/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/content/stelastory.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/content/stelastory.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/modal1.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/modal1.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/modal2.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/modal2.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/modal3.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/modal3.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/developer/data-update/modal4.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/developer/data-update/modal4.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/developer/home.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/developer/home.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/billing/invoice.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/billing/invoice.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/contact/message_notification.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/contact/message_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/contact/support_notification.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/contact/support_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/billing_payment.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/billing_payment.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/charges.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/charges.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/payment_notification.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/payment_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/sale_notification.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/sale_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/payments/withdrawals.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/payments/withdrawals.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/emails-template/support/support_notification.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/emails-template/support/support_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/home.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/home.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/inbox/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/inbox/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/inventory/resources/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/inventory/resources/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/inventory/services/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/inventory/services/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/jobs/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/jobs/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/aboutstela/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/aboutstela/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/appstela/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/appstela/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/billing/form-billing.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/billing/form-billing.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/billing/recipt-data.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/billing/recipt-data.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/blog-feed.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/blog-feed.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/categories/modal4.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/categories/modal4.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/chatbox.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/chatbox.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/chatbox2.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/chatbox2.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/colors/modal2.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/colors/modal2.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/contact/form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/contact/form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/contact/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/contact/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/dynamic-formset.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/dynamic-formset.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/form-base.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/form-base.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/formset-base-services.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/formset-base-services.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/formset-base.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/formset-base.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/formset.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/formset.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages-v1.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages-v1.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/instagram-alert.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/instagram-alert.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/community/formdata.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/community/formdata.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/newcomer/form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/newcomer/form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/post/list-modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/post/list-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/post/main-modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/post/main-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/catalog-modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/catalog-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/catalog-form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/catalog-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/category-form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/category-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/color-form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/color-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/product-form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/product-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/new/size-form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/new/size-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/product-modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/product-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/size-modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/size-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/products/update/product-form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/products/update/product-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/profile/dynamic-form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/profile/dynamic-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/projects/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/projects/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/single-form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/single-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/staff/form.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/staff/form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stela_story/feed-item.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stela_story/feed-item.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelafooter/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelafooter/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelamedia/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelamedia/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/stelapath/modal.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/stelapath/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/bank_statements.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/bank_statements.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/invoices.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/invoices.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/retentions.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/retentions.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/load-data/tables/tax-return.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/load-data/tables/tax-return.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/email-marketing/email_list.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/email-marketing/email_list.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/newcomer.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/newcomer.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/orders/list_view.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/orders/list_view.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/orders/order_update.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/orders/order_update.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/payments/homebrew.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/payments/homebrew.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/payments/register-wallet.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/payments/register-wallet.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/payments/wallet-list.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/payments/wallet-list.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/payments/withdraw.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/payments/withdraw.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/prostela-expert/index.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/prostela-expert/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/reviews/reviews.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/reviews/reviews.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/support/case-detail.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/support/case-detail.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/support/list.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/support/list.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/users/profile.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/users/profile.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/users/users-control.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/users/users-control.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templates/stela_control/users/users.html` & `stela_professional-0.4.3/stela_control/templates/stela_control/users/users.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/templatetags/stelatags.py` & `stela_professional-0.4.3/stela_control/templatetags/stelatags.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/tokenize.py` & `stela_professional-0.4.3/stela_control/tokenize.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/urls.py` & `stela_professional-0.4.3/stela_control/urls.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_control/views.py` & `stela_professional-0.4.3/stela_control/views.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.2/stela_professional.egg-info/PKG-INFO` & `stela_professional-0.4.3/stela_professional.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stela_professional
-Version: 0.4.2
+Version: 0.4.3
 Summary: All apps in one for business.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stela_professional-0.4.2/stela_professional.egg-info/SOURCES.txt` & `stela_professional-0.4.3/stela_professional.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 stela_control/templates/stela_control/load-data/blog-feed.html
 stela_control/templates/stela_control/load-data/chatbox.html
 stela_control/templates/stela_control/load-data/chatbox2.html
 stela_control/templates/stela_control/load-data/city_data.html
 stela_control/templates/stela_control/load-data/dynamic-formset.html
 stela_control/templates/stela_control/load-data/form-base.html
 stela_control/templates/stela_control/load-data/form-errors.html
+stela_control/templates/stela_control/load-data/form.html
 stela_control/templates/stela_control/load-data/formset-base-services.html
 stela_control/templates/stela_control/load-data/formset-base.html
 stela_control/templates/stela_control/load-data/formset.html
 stela_control/templates/stela_control/load-data/hashtags.html
 stela_control/templates/stela_control/load-data/instagram-alert.html
 stela_control/templates/stela_control/load-data/remove-complete.html
 stela_control/templates/stela_control/load-data/single-form.html
```

