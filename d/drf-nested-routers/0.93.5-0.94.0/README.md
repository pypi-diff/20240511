# Comparing `tmp/drf-nested-routers-0.93.5.tar.gz` & `tmp/drf-nested-routers-0.94.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-nested-routers-0.93.5.tar", last modified: Tue Dec 19 23:25:19 2023, max compression
+gzip compressed data, was "drf-nested-routers-0.94.0.tar", last modified: Fri May 10 13:55:12 2024, max compression
```

## Comparing `drf-nested-routers-0.93.5.tar` & `drf-nested-routers-0.94.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 alanjds   (1000) alanjds   (1000)        0 2023-12-19 23:25:19.469170 drf-nested-routers-0.93.5/
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)    10267 2020-02-15 01:55:23.000000 drf-nested-routers-0.93.5/LICENSE
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)      132 2020-02-15 01:55:23.000000 drf-nested-routers-0.93.5/MANIFEST.in
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)    13957 2023-12-19 23:25:19.469170 drf-nested-routers-0.93.5/PKG-INFO
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)    10452 2023-12-19 23:22:43.000000 drf-nested-routers-0.93.5/README.md
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)      610 2020-02-15 01:55:23.000000 drf-nested-routers-0.93.5/README.rst
-drwxrwxr-x   0 alanjds   (1000) alanjds   (1000)        0 2023-12-19 23:25:19.469170 drf-nested-routers-0.93.5/drf_nested_routers.egg-info/
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)    13957 2023-12-19 23:25:19.000000 drf-nested-routers-0.93.5/drf_nested_routers.egg-info/PKG-INFO
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)      672 2023-12-19 23:25:19.000000 drf-nested-routers-0.93.5/drf_nested_routers.egg-info/SOURCES.txt
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)        1 2023-12-19 23:25:19.000000 drf-nested-routers-0.93.5/drf_nested_routers.egg-info/dependency_links.txt
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)       40 2023-12-19 23:25:19.000000 drf-nested-routers-0.93.5/drf_nested_routers.egg-info/requires.txt
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)       53 2023-12-19 23:25:19.000000 drf-nested-routers-0.93.5/drf_nested_routers.egg-info/top_level.txt
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)      129 2023-12-19 23:22:43.000000 drf-nested-routers-0.93.5/requirements.txt
-drwxrwxr-x   0 alanjds   (1000) alanjds   (1000)        0 2023-12-19 23:25:19.469170 drf-nested-routers-0.93.5/rest_framework_nested/
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)      631 2023-12-19 23:23:54.000000 drf-nested-routers-0.93.5/rest_framework_nested/__init__.py
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     4323 2021-03-12 19:37:55.000000 drf-nested-routers-0.93.5/rest_framework_nested/relations.py
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     5958 2022-10-21 20:34:05.000000 drf-nested-routers-0.93.5/rest_framework_nested/routers.py
-drwxrwxr-x   0 alanjds   (1000) alanjds   (1000)        0 2023-12-19 23:25:19.469170 drf-nested-routers-0.93.5/rest_framework_nested/runtests/
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)        0 2020-02-15 01:55:23.000000 drf-nested-routers-0.93.5/rest_framework_nested/runtests/__init__.py
--rwxr-xr-x   0 alanjds   (1000) alanjds   (1000)     2762 2020-02-15 01:55:23.000000 drf-nested-routers-0.93.5/rest_framework_nested/runtests/runcoverage.py
--rwxr-xr-x   0 alanjds   (1000) alanjds   (1000)     1379 2020-02-15 01:55:23.000000 drf-nested-routers-0.93.5/rest_framework_nested/runtests/runtests.py
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     4833 2023-12-19 23:22:43.000000 drf-nested-routers-0.93.5/rest_framework_nested/runtests/settings.py
--rw-r--r--   0 alanjds   (1000) alanjds   (1000)      126 2020-02-15 01:55:23.000000 drf-nested-routers-0.93.5/rest_framework_nested/runtests/urls.py
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     2078 2021-03-12 19:37:55.000000 drf-nested-routers-0.93.5/rest_framework_nested/serializers.py
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     2744 2023-12-19 23:22:43.000000 drf-nested-routers-0.93.5/rest_framework_nested/viewsets.py
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)      221 2023-12-19 23:25:19.469170 drf-nested-routers-0.93.5/setup.cfg
--rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     3166 2023-12-19 23:22:43.000000 drf-nested-routers-0.93.5/setup.py
+drwxrwxr-x   0 alanjds   (1000) alanjds   (1000)        0 2024-05-10 13:55:12.483011 drf-nested-routers-0.94.0/
+-rw-r--r--   0 alanjds   (1000) alanjds   (1000)    10267 2020-02-15 01:55:23.000000 drf-nested-routers-0.94.0/LICENSE
+-rw-r--r--   0 alanjds   (1000) alanjds   (1000)      132 2020-02-15 01:55:23.000000 drf-nested-routers-0.94.0/MANIFEST.in
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)    11536 2024-05-10 13:55:12.483011 drf-nested-routers-0.94.0/PKG-INFO
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)    10456 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/README.md
+drwxrwxr-x   0 alanjds   (1000) alanjds   (1000)        0 2024-05-10 13:55:12.483011 drf-nested-routers-0.94.0/drf_nested_routers.egg-info/
+-rw-r--r--   0 alanjds   (1000) alanjds   (1000)    11536 2024-05-10 13:55:12.000000 drf-nested-routers-0.94.0/drf_nested_routers.egg-info/PKG-INFO
+-rw-r--r--   0 alanjds   (1000) alanjds   (1000)      661 2024-05-10 13:55:12.000000 drf-nested-routers-0.94.0/drf_nested_routers.egg-info/SOURCES.txt
+-rw-r--r--   0 alanjds   (1000) alanjds   (1000)        1 2024-05-10 13:55:12.000000 drf-nested-routers-0.94.0/drf_nested_routers.egg-info/dependency_links.txt
+-rw-r--r--   0 alanjds   (1000) alanjds   (1000)       40 2024-05-10 13:55:12.000000 drf-nested-routers-0.94.0/drf_nested_routers.egg-info/requires.txt
+-rw-r--r--   0 alanjds   (1000) alanjds   (1000)       53 2024-05-10 13:55:12.000000 drf-nested-routers-0.94.0/drf_nested_routers.egg-info/top_level.txt
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)      129 2023-12-19 23:22:43.000000 drf-nested-routers-0.94.0/requirements.txt
+drwxrwxr-x   0 alanjds   (1000) alanjds   (1000)        0 2024-05-10 13:55:12.483011 drf-nested-routers-0.94.0/rest_framework_nested/
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)      631 2024-05-10 13:53:50.000000 drf-nested-routers-0.94.0/rest_framework_nested/__init__.py
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     4523 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/rest_framework_nested/relations.py
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     6090 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/rest_framework_nested/routers.py
+drwxrwxr-x   0 alanjds   (1000) alanjds   (1000)        0 2024-05-10 13:55:12.483011 drf-nested-routers-0.94.0/rest_framework_nested/runtests/
+-rw-r--r--   0 alanjds   (1000) alanjds   (1000)        0 2020-02-15 01:55:23.000000 drf-nested-routers-0.94.0/rest_framework_nested/runtests/__init__.py
+-rwxrwxr-x   0 alanjds   (1000) alanjds   (1000)     2857 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/rest_framework_nested/runtests/runcoverage.py
+-rwxrwxr-x   0 alanjds   (1000) alanjds   (1000)     1426 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/rest_framework_nested/runtests/runtests.py
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     4869 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/rest_framework_nested/runtests/settings.py
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)      156 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/rest_framework_nested/runtests/urls.py
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     2402 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/rest_framework_nested/serializers.py
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     3396 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/rest_framework_nested/viewsets.py
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)      221 2024-05-10 13:55:12.483011 drf-nested-routers-0.94.0/setup.cfg
+-rw-rw-r--   0 alanjds   (1000) alanjds   (1000)     3130 2024-05-10 13:53:24.000000 drf-nested-routers-0.94.0/setup.py
```

### Comparing `drf-nested-routers-0.93.5/LICENSE` & `drf-nested-routers-0.94.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-nested-routers-0.93.5/PKG-INFO` & `drf-nested-routers-0.94.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,319 +1,15 @@
 Metadata-Version: 2.1
 Name: drf-nested-routers
-Version: 0.93.5
+Version: 0.94.0
 Summary: Nested resources for the Django Rest Framework
 Home-page: https://github.com/alanjds/drf-nested-routers
 Author: Alan Justino et al.
 Author-email: alan.justino@yahoo.com.br
 License: Apache
-Description: **This is a work in progress. It "works for me" at www.apiregistro.com.br,
-        but I cannot warranty that it fully "works everywhere" yet. Join us on Gitter (below) if you need some help.**
-        
-        # drf-nested-routers
-        
-        [![Join the chat at https://gitter.im/alanjds/drf-nested-routers](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/alanjds/drf-nested-routers?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-        [![Build Status](https://github.com/alanjds/drf-nested-routers/workflows/CI/badge.svg)](https://github.com/alanjds/drf-nested-routers/actions?query=workflow%3ACI+branch%3Amaster)
-        
-        This package provides routers and fields to create nested resources in the [Django Rest Framework](http://django-rest-framework.org/)
-        
-        Nested resources are needed for full REST URL structure, if one resource lives inside another.
-        
-        The following example is about Domains and DNS Nameservers.
-        There are many domains, and each domain has many nameservers. The "nameserver" resource does not
-        exist without a domain, so you need it "nested" inside the domain.
-        
-        
-        ## Requirements & Compatibility
-        
-        -  Python (3.8, 3.9, 3.10, 3.11)
-        -  Django (3.2, 4.1, 4.2)
-        -  Django REST Framework (3.14)
-        
-        It may work with lower versions, but since the release **0.93.5** is no more tested on CI for Python 3.6 or lower.<br/>
-        And since **0.92.1** is no more tested on CI for Pythons 2.7 to 3.5, Django 1.11 to 2.1 or DRF 3.6 to 3.10.<br/>
-        Before that, the release **0.90.2** was tested also with DRF 2.4.3 up to 3.7.
-        
-        
-        ## Installation
-        
-        You can install this library using pip:
-        
-        ```pip install drf-nested-routers```
-        
-        It is not needed to add this library in your Django project's `settings.py` file, as it does not contain any app, signal or model.
-        
-        ## Quickstart
-        
-        The desired URL signatures are:
-        ```
-        /domain/ <- Domains list
-        /domain/{pk}/ <- One domain, from {pk}
-        /domain/{domain_pk}/nameservers/ <- Nameservers of domain from {domain_pk}
-        /domain/{domain_pk}/nameservers/{pk} <- Specific nameserver from {pk}, of domain from {domain_pk}
-        ```
-        
-        How to do it (example):
-        ```python
-        # urls.py
-        from rest_framework_nested import routers
-        from views import DomainViewSet, NameserverViewSet
-        (...)
-        
-        router = routers.SimpleRouter()
-        router.register(r'domains', DomainViewSet)
-        
-        domains_router = routers.NestedSimpleRouter(router, r'domains', lookup='domain')
-        domains_router.register(r'nameservers', NameserverViewSet, basename='domain-nameservers')
-        # 'basename' is optional. Needed only if the same viewset is registered more than once
-        # Official DRF docs on this option: http://www.django-rest-framework.org/api-guide/routers/
-        
-        urlpatterns = [
-            path(r'', include(router.urls)),
-            path(r'', include(domains_router.urls)),
-        ]
-        ```
-        
-        ```python
-        # views.py
-        
-        ## For Django' ORM-based resources ##
-        
-        class NameserverViewSet(viewsets.ModelViewSet):
-            def get_queryset(self):
-                return Nameserver.objects.filter(domain=self.kwargs['domain_pk'])
-        
-        ## OR: non-ORM resources ##
-        
-        class NameserverViewSet(viewsets.ViewSet):
-            def list(self, request, domain_pk=None):
-                nameservers = self.queryset.filter(domain=domain_pk)
-                (...)
-                return Response([...])
-        
-            def retrieve(self, request, pk=None, domain_pk=None):
-                nameservers = self.queryset.get(pk=pk, domain=domain_pk)
-                (...)
-                return Response(serializer.data)
-        ```
-        
-        ## Advanced
-        
-        ### Hyperlinks for Nested resources
-        
-        **(optional)** If you need hyperlinks for nested relations, you need a custom serializer.
-        
-        There you will inform how to access the *parent* of the instance being serialized when
-        building the *children* URL.
-        
-        In the following example, an instance of Nameserver on `/domain/{domain_pk}/nameservers/{pk}`
-        is being informed that the *parent* Domain should be looked up using the `domain_pk` kwarg
-        from the URL:
-        ```python
-        # serializers.py
-        # (needed only if you want hyperlinks for nested relations on API)
-        from rest_framework_nested.relations import NestedHyperlinkedRelatedField
-        
-        class DomainSerializer(HyperlinkedModelSerializer):
-            class Meta:
-                model = Domain
-        
-            nameservers = HyperlinkedIdentityField(
-                view_name='domain-nameservers-list',
-                lookup_url_kwarg='domain_pk'
-                                # ^-- Nameserver queryset will .get(domain_pk=domain_pk)
-                                #     being this value from URL kwargs
-            )
-        
-        	## OR ##
-        
-            nameservers = NestedHyperlinkedRelatedField(
-                many=True,
-                read_only=True,   # Or add a queryset
-                view_name='domain-nameservers-detail',
-                parent_lookup_kwargs={'domain_pk': 'domain__pk'}
-                                    # ^-- Nameserver queryset will .filter(domain__pk=domain_pk)
-                                    #     being domain_pk (ONE underscore) value from URL kwargs
-            )
-        ```
-        
-        **(optional)** If you want a little bit more control over the fields displayed for the nested relations while looking at the parent, you need a custom serializer using NestedHyperlinkedModelSerializer.
-        ```python
-        from rest_framework.serializers import HyperlinkedModelSerializer
-        from rest_framework_nested.serializers import NestedHyperlinkedModelSerializer
-        
-        class NameserverSerializers(HyperlinkedModelSerializer):
-        	class Meta:
-        		model = Nameserver
-        		fields = (...)
-        
-        
-        class DomainNameserverSerializers(NestedHyperlinkedModelSerializer):
-        	parent_lookup_kwargs = {
-        		'domain_pk': 'domain__pk',
-        	}
-        	class Meta:
-        		model = Nameserver
-        		fields = ('url', ...)
-        
-        
-        class DomainSerializer(HyperlinkedModelSerializer):
-        	class Meta:
-        		model = Domain
-        		fields = (..., 'nameservers')
-        
-        	nameservers = DomainNameserverSerializers(many=True, read_only=True)
-        ```
-        
-        ### Infinite-depth Nesting
-        
-        Example of nested router 3 levels deep.
-        You can use this same logic to nest routers as deep as you need.
-        This example ahead accomplishes the below URL patterns.
-        ```
-        /clients/
-        /clients/{pk}/
-        /clients/{client_pk}/maildrops/
-        /clients/{client_pk}/maildrops/{pk}/
-        /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/
-        /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/{pk}/
-        ```
-        
-        ```python
-        # urls.py
-        router = DefaultRouter()
-        router.register(r'clients', ClientViewSet, basename='clients')
-        ## generates:
-        # /clients/
-        # /clients/{pk}/
-        
-        client_router = routers.NestedSimpleRouter(router, r'clients', lookup='client')
-        client_router.register(r'maildrops', MailDropViewSet, basename='maildrops')
-        ## generates:
-        # /clients/{client_pk}/maildrops/
-        # /clients/{client_pk}/maildrops/{pk}/
-        
-        maildrops_router = routers.NestedSimpleRouter(client_router, r'maildrops', lookup='maildrop')
-        maildrops_router.register(r'recipients', MailRecipientViewSet, basename='recipients')
-        ## generates:
-        # /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/
-        # /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/{pk}/
-        
-        urlpatterns = [
-            path(r'', include(router.urls)),
-            path(r'', include(client_router.urls)),
-            path(r'', include(maildrops_router.urls)),
-        ]
-        ```
-        
-        ```python
-        # views.py
-        class ClientViewSet(viewsets.ViewSet):
-            serializer_class = ClientSerializer
-        
-            def list(self, request,):
-                queryset = Client.objects.filter()
-                serializer = ClientSerializer(queryset, many=True)
-                return Response(serializer.data)
-        
-            def retrieve(self, request, pk=None):
-                queryset = Client.objects.filter()
-                client = get_object_or_404(queryset, pk=pk)
-                serializer = ClientSerializer(client)
-                return Response(serializer.data)
-        
-        
-        class MailDropViewSet(viewsets.ViewSet):
-            serializer_class = MailDropSerializer
-        
-            def list(self, request, client_pk=None):
-                queryset = MailDrop.objects.filter(client=client_pk)
-                serializer = MailDropSerializer(queryset, many=True)
-                return Response(serializer.data)
-        
-            def retrieve(self, request, pk=None, client_pk=None):
-                queryset = MailDrop.objects.filter(pk=pk, client=client_pk)
-                maildrop = get_object_or_404(queryset, pk=pk)
-                serializer = MailDropSerializer(maildrop)
-                return Response(serializer.data)
-        
-        
-        class MailRecipientViewSet(viewsets.ViewSet):
-            serializer_class = MailRecipientSerializer
-        
-            def list(self, request, client_pk=None, maildrop_pk=None):
-                queryset = MailRecipient.objects.filter(mail_drop__client=client_pk, mail_drop=maildrop_pk)
-                serializer = MailRecipientSerializer(queryset, many=True)
-                return Response(serializer.data)
-        
-            def retrieve(self, request, pk=None, client_pk=None, maildrop_pk=None):
-                queryset = MailRecipient.objects.filter(pk=pk, mail_drop=maildrop_pk, mail_drop__client=client_pk)
-                maildrop = get_object_or_404(queryset, pk=pk)
-                serializer = MailRecipientSerializer(maildrop)
-                return Response(serializer.data)
-        ```
-        
-        ```python
-        # serializers.py
-        class ClientSerializer(HyperlinkedModelSerializer):
-            class Meta:
-                model = Client
-                fields = (...)
-        
-        
-        class MailDropSerializer(NestedHyperlinkedModelSerializer):
-            parent_lookup_kwargs = {
-                'client_pk': 'client__pk',
-            }
-            class Meta:
-                model = MailDrop
-                fields = (...)
-        
-        
-        class MailRecipientSerializer(NestedHyperlinkedModelSerializer):
-            parent_lookup_kwargs = {
-                'maildrop_pk': 'mail_drop__pk',
-                'client_pk': 'mail_drop__client__pk',
-            }
-            class Meta:
-                model = MailRecipient
-                fields = (...)
-        ```
-        
-        ## Testing
-        
-        In order to get started with testing, you will need to install [tox](https://tox.readthedocs.io/en/latest/).
-        Once installed, you can then run one environment locally, to speed up your development cycle:
-        
-        ```
-        $ tox -e py39-django3.1-drf3.11
-        ```
-        
-        Once you submit a pull request, your changes will be run against many environments with GitHub Actions named CI.
-        
-        
-        ## License
-        
-        This package is licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-        and can undestand more at http://choosealicense.com/licenses/apache/ on the
-        sidebar notes.
-        
-        Apache Licence v2.0 is a MIT-like licence. This means, in plain English:
-        - It's truly open source
-        - You can use it as you wish, for money or not
-        - You can sublicence it (change the licence!!)
-        - This way, you can even use it on your closed-source project
-        As long as:
-        - You cannot use the authors name, logos, etc, to endorse a project
-        - You keep the authors copyright notices where this code got used, even on your closed-source project
-        (come on, even Microsoft kept BSD notices on Windows about its TCP/IP stack :P)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
@@ -324,7 +20,311 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+**This is a work in progress. It "works for me" at www.apiregistro.com.br,
+but I cannot warranty that it fully "works everywhere" yet. Join us on Gitter (below) if you need some help.**
+
+# drf-nested-routers
+
+[![Join the chat at https://gitter.im/alanjds/drf-nested-routers](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/alanjds/drf-nested-routers?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Build Status](https://github.com/alanjds/drf-nested-routers/workflows/CI/badge.svg)](https://github.com/alanjds/drf-nested-routers/actions?query=workflow%3ACI+branch%3Amaster)
+
+This package provides routers and fields to create nested resources in the [Django Rest Framework](http://django-rest-framework.org/)
+
+Nested resources are needed for full REST URL structure, if one resource lives inside another.
+
+The following example is about Domains and DNS Nameservers.
+There are many domains, and each domain has many nameservers. The "nameserver" resource does not
+exist without a domain, so you need it "nested" inside the domain.
+
+
+## Requirements & Compatibility
+
+-  Python (3.8, 3.9, 3.10, 3.11)
+-  Django (3.2, 4.1, 4.2)
+-  Django REST Framework (3.14)
+
+It may work with lower versions, but since the release **0.93.5** is no more tested on CI for Python 3.6 or lower.<br/>
+And since **0.92.1** is no more tested on CI for Pythons 2.7 to 3.5, Django 1.11 to 2.1 or DRF 3.6 to 3.10.<br/>
+Before that, the release **0.90.2** was tested also with DRF 2.4.3 up to 3.7.
+
+
+## Installation
+
+You can install this library using pip:
+
+```pip install drf-nested-routers```
+
+It is not needed to add this library in your Django project's `settings.py` file, as it does not contain any app, signal or model.
+
+## Quickstart
+
+The desired URL signatures are:
+```
+/domains/ <- Domains list
+/domains/{pk}/ <- One domain, from {pk}
+/domains/{domain_pk}/nameservers/ <- Nameservers of domain from {domain_pk}
+/domains/{domain_pk}/nameservers/{pk} <- Specific nameserver from {pk}, of domain from {domain_pk}
+```
+
+How to do it (example):
+```python
+# urls.py
+from rest_framework_nested import routers
+from views import DomainViewSet, NameserverViewSet
+(...)
+
+router = routers.SimpleRouter()
+router.register(r'domains', DomainViewSet)
+
+domains_router = routers.NestedSimpleRouter(router, r'domains', lookup='domain')
+domains_router.register(r'nameservers', NameserverViewSet, basename='domain-nameservers')
+# 'basename' is optional. Needed only if the same viewset is registered more than once
+# Official DRF docs on this option: http://www.django-rest-framework.org/api-guide/routers/
+
+urlpatterns = [
+    path(r'', include(router.urls)),
+    path(r'', include(domains_router.urls)),
+]
+```
+
+```python
+# views.py
+
+## For Django' ORM-based resources ##
+
+class NameserverViewSet(viewsets.ModelViewSet):
+    def get_queryset(self):
+        return Nameserver.objects.filter(domain=self.kwargs['domain_pk'])
+
+## OR: non-ORM resources ##
+
+class NameserverViewSet(viewsets.ViewSet):
+    def list(self, request, domain_pk=None):
+        nameservers = self.queryset.filter(domain=domain_pk)
+        (...)
+        return Response([...])
+
+    def retrieve(self, request, pk=None, domain_pk=None):
+        nameservers = self.queryset.get(pk=pk, domain=domain_pk)
+        (...)
+        return Response(serializer.data)
+```
+
+## Advanced
+
+### Hyperlinks for Nested resources
+
+**(optional)** If you need hyperlinks for nested relations, you need a custom serializer.
+
+There you will inform how to access the *parent* of the instance being serialized when
+building the *children* URL.
+
+In the following example, an instance of Nameserver on `/domain/{domain_pk}/nameservers/{pk}`
+is being informed that the *parent* Domain should be looked up using the `domain_pk` kwarg
+from the URL:
+```python
+# serializers.py
+# (needed only if you want hyperlinks for nested relations on API)
+from rest_framework_nested.relations import NestedHyperlinkedRelatedField
+
+class DomainSerializer(HyperlinkedModelSerializer):
+    class Meta:
+        model = Domain
+
+    nameservers = HyperlinkedIdentityField(
+        view_name='domain-nameservers-list',
+        lookup_url_kwarg='domain_pk'
+                        # ^-- Nameserver queryset will .get(domain_pk=domain_pk)
+                        #     being this value from URL kwargs
+    )
+
+	## OR ##
+
+    nameservers = NestedHyperlinkedRelatedField(
+        many=True,
+        read_only=True,   # Or add a queryset
+        view_name='domain-nameservers-detail',
+        parent_lookup_kwargs={'domain_pk': 'domain__pk'}
+                            # ^-- Nameserver queryset will .filter(domain__pk=domain_pk)
+                            #     being domain_pk (ONE underscore) value from URL kwargs
+    )
+```
+
+**(optional)** If you want a little bit more control over the fields displayed for the nested relations while looking at the parent, you need a custom serializer using NestedHyperlinkedModelSerializer.
+```python
+from rest_framework.serializers import HyperlinkedModelSerializer
+from rest_framework_nested.serializers import NestedHyperlinkedModelSerializer
+
+class NameserverSerializers(HyperlinkedModelSerializer):
+	class Meta:
+		model = Nameserver
+		fields = (...)
+
+
+class DomainNameserverSerializers(NestedHyperlinkedModelSerializer):
+	parent_lookup_kwargs = {
+		'domain_pk': 'domain__pk',
+	}
+	class Meta:
+		model = Nameserver
+		fields = ('url', ...)
+
+
+class DomainSerializer(HyperlinkedModelSerializer):
+	class Meta:
+		model = Domain
+		fields = (..., 'nameservers')
+
+	nameservers = DomainNameserverSerializers(many=True, read_only=True)
+```
+
+### Infinite-depth Nesting
+
+Example of nested router 3 levels deep.
+You can use this same logic to nest routers as deep as you need.
+This example ahead accomplishes the below URL patterns.
+```
+/clients/
+/clients/{pk}/
+/clients/{client_pk}/maildrops/
+/clients/{client_pk}/maildrops/{pk}/
+/clients/{client_pk}/maildrops/{maildrop_pk}/recipients/
+/clients/{client_pk}/maildrops/{maildrop_pk}/recipients/{pk}/
+```
+
+```python
+# urls.py
+router = DefaultRouter()
+router.register(r'clients', ClientViewSet, basename='clients')
+## generates:
+# /clients/
+# /clients/{pk}/
+
+client_router = routers.NestedSimpleRouter(router, r'clients', lookup='client')
+client_router.register(r'maildrops', MailDropViewSet, basename='maildrops')
+## generates:
+# /clients/{client_pk}/maildrops/
+# /clients/{client_pk}/maildrops/{pk}/
+
+maildrops_router = routers.NestedSimpleRouter(client_router, r'maildrops', lookup='maildrop')
+maildrops_router.register(r'recipients', MailRecipientViewSet, basename='recipients')
+## generates:
+# /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/
+# /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/{pk}/
+
+urlpatterns = [
+    path(r'', include(router.urls)),
+    path(r'', include(client_router.urls)),
+    path(r'', include(maildrops_router.urls)),
+]
+```
+
+```python
+# views.py
+class ClientViewSet(viewsets.ViewSet):
+    serializer_class = ClientSerializer
+
+    def list(self, request,):
+        queryset = Client.objects.filter()
+        serializer = ClientSerializer(queryset, many=True)
+        return Response(serializer.data)
+
+    def retrieve(self, request, pk=None):
+        queryset = Client.objects.filter()
+        client = get_object_or_404(queryset, pk=pk)
+        serializer = ClientSerializer(client)
+        return Response(serializer.data)
+
+
+class MailDropViewSet(viewsets.ViewSet):
+    serializer_class = MailDropSerializer
+
+    def list(self, request, client_pk=None):
+        queryset = MailDrop.objects.filter(client=client_pk)
+        serializer = MailDropSerializer(queryset, many=True)
+        return Response(serializer.data)
+
+    def retrieve(self, request, pk=None, client_pk=None):
+        queryset = MailDrop.objects.filter(pk=pk, client=client_pk)
+        maildrop = get_object_or_404(queryset, pk=pk)
+        serializer = MailDropSerializer(maildrop)
+        return Response(serializer.data)
+
+
+class MailRecipientViewSet(viewsets.ViewSet):
+    serializer_class = MailRecipientSerializer
+
+    def list(self, request, client_pk=None, maildrop_pk=None):
+        queryset = MailRecipient.objects.filter(mail_drop__client=client_pk, mail_drop=maildrop_pk)
+        serializer = MailRecipientSerializer(queryset, many=True)
+        return Response(serializer.data)
+
+    def retrieve(self, request, pk=None, client_pk=None, maildrop_pk=None):
+        queryset = MailRecipient.objects.filter(pk=pk, mail_drop=maildrop_pk, mail_drop__client=client_pk)
+        maildrop = get_object_or_404(queryset, pk=pk)
+        serializer = MailRecipientSerializer(maildrop)
+        return Response(serializer.data)
+```
+
+```python
+# serializers.py
+class ClientSerializer(HyperlinkedModelSerializer):
+    class Meta:
+        model = Client
+        fields = (...)
+
+
+class MailDropSerializer(NestedHyperlinkedModelSerializer):
+    parent_lookup_kwargs = {
+        'client_pk': 'client__pk',
+    }
+    class Meta:
+        model = MailDrop
+        fields = (...)
+
+
+class MailRecipientSerializer(NestedHyperlinkedModelSerializer):
+    parent_lookup_kwargs = {
+        'maildrop_pk': 'mail_drop__pk',
+        'client_pk': 'mail_drop__client__pk',
+    }
+    class Meta:
+        model = MailRecipient
+        fields = (...)
+```
+
+## Testing
+
+In order to get started with testing, you will need to install [tox](https://tox.readthedocs.io/en/latest/).
+Once installed, you can then run one environment locally, to speed up your development cycle:
+
+```
+$ tox -e py39-django3.1-drf3.11
+```
+
+Once you submit a pull request, your changes will be run against many environments with GitHub Actions named CI.
+
+
+## License
+
+This package is licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+and can undestand more at http://choosealicense.com/licenses/apache/ on the
+sidebar notes.
+
+Apache Licence v2.0 is a MIT-like licence. This means, in plain English:
+- It's truly open source
+- You can use it as you wish, for money or not
+- You can sublicence it (change the licence!!)
+- This way, you can even use it on your closed-source project
+As long as:
+- You cannot use the authors name, logos, etc, to endorse a project
+- You keep the authors copyright notices where this code got used, even on your closed-source project
+(come on, even Microsoft kept BSD notices on Windows about its TCP/IP stack :P)
```

### Comparing `drf-nested-routers-0.93.5/README.md` & `drf-nested-routers-0.94.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 
 It is not needed to add this library in your Django project's `settings.py` file, as it does not contain any app, signal or model.
 
 ## Quickstart
 
 The desired URL signatures are:
 ```
-/domain/ <- Domains list
-/domain/{pk}/ <- One domain, from {pk}
-/domain/{domain_pk}/nameservers/ <- Nameservers of domain from {domain_pk}
-/domain/{domain_pk}/nameservers/{pk} <- Specific nameserver from {pk}, of domain from {domain_pk}
+/domains/ <- Domains list
+/domains/{pk}/ <- One domain, from {pk}
+/domains/{domain_pk}/nameservers/ <- Nameservers of domain from {domain_pk}
+/domains/{domain_pk}/nameservers/{pk} <- Specific nameserver from {pk}, of domain from {domain_pk}
 ```
 
 How to do it (example):
 ```python
 # urls.py
 from rest_framework_nested import routers
 from views import DomainViewSet, NameserverViewSet
```

### Comparing `drf-nested-routers-0.93.5/drf_nested_routers.egg-info/PKG-INFO` & `drf-nested-routers-0.94.0/drf_nested_routers.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,319 +1,15 @@
 Metadata-Version: 2.1
 Name: drf-nested-routers
-Version: 0.93.5
+Version: 0.94.0
 Summary: Nested resources for the Django Rest Framework
 Home-page: https://github.com/alanjds/drf-nested-routers
 Author: Alan Justino et al.
 Author-email: alan.justino@yahoo.com.br
 License: Apache
-Description: **This is a work in progress. It "works for me" at www.apiregistro.com.br,
-        but I cannot warranty that it fully "works everywhere" yet. Join us on Gitter (below) if you need some help.**
-        
-        # drf-nested-routers
-        
-        [![Join the chat at https://gitter.im/alanjds/drf-nested-routers](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/alanjds/drf-nested-routers?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-        [![Build Status](https://github.com/alanjds/drf-nested-routers/workflows/CI/badge.svg)](https://github.com/alanjds/drf-nested-routers/actions?query=workflow%3ACI+branch%3Amaster)
-        
-        This package provides routers and fields to create nested resources in the [Django Rest Framework](http://django-rest-framework.org/)
-        
-        Nested resources are needed for full REST URL structure, if one resource lives inside another.
-        
-        The following example is about Domains and DNS Nameservers.
-        There are many domains, and each domain has many nameservers. The "nameserver" resource does not
-        exist without a domain, so you need it "nested" inside the domain.
-        
-        
-        ## Requirements & Compatibility
-        
-        -  Python (3.8, 3.9, 3.10, 3.11)
-        -  Django (3.2, 4.1, 4.2)
-        -  Django REST Framework (3.14)
-        
-        It may work with lower versions, but since the release **0.93.5** is no more tested on CI for Python 3.6 or lower.<br/>
-        And since **0.92.1** is no more tested on CI for Pythons 2.7 to 3.5, Django 1.11 to 2.1 or DRF 3.6 to 3.10.<br/>
-        Before that, the release **0.90.2** was tested also with DRF 2.4.3 up to 3.7.
-        
-        
-        ## Installation
-        
-        You can install this library using pip:
-        
-        ```pip install drf-nested-routers```
-        
-        It is not needed to add this library in your Django project's `settings.py` file, as it does not contain any app, signal or model.
-        
-        ## Quickstart
-        
-        The desired URL signatures are:
-        ```
-        /domain/ <- Domains list
-        /domain/{pk}/ <- One domain, from {pk}
-        /domain/{domain_pk}/nameservers/ <- Nameservers of domain from {domain_pk}
-        /domain/{domain_pk}/nameservers/{pk} <- Specific nameserver from {pk}, of domain from {domain_pk}
-        ```
-        
-        How to do it (example):
-        ```python
-        # urls.py
-        from rest_framework_nested import routers
-        from views import DomainViewSet, NameserverViewSet
-        (...)
-        
-        router = routers.SimpleRouter()
-        router.register(r'domains', DomainViewSet)
-        
-        domains_router = routers.NestedSimpleRouter(router, r'domains', lookup='domain')
-        domains_router.register(r'nameservers', NameserverViewSet, basename='domain-nameservers')
-        # 'basename' is optional. Needed only if the same viewset is registered more than once
-        # Official DRF docs on this option: http://www.django-rest-framework.org/api-guide/routers/
-        
-        urlpatterns = [
-            path(r'', include(router.urls)),
-            path(r'', include(domains_router.urls)),
-        ]
-        ```
-        
-        ```python
-        # views.py
-        
-        ## For Django' ORM-based resources ##
-        
-        class NameserverViewSet(viewsets.ModelViewSet):
-            def get_queryset(self):
-                return Nameserver.objects.filter(domain=self.kwargs['domain_pk'])
-        
-        ## OR: non-ORM resources ##
-        
-        class NameserverViewSet(viewsets.ViewSet):
-            def list(self, request, domain_pk=None):
-                nameservers = self.queryset.filter(domain=domain_pk)
-                (...)
-                return Response([...])
-        
-            def retrieve(self, request, pk=None, domain_pk=None):
-                nameservers = self.queryset.get(pk=pk, domain=domain_pk)
-                (...)
-                return Response(serializer.data)
-        ```
-        
-        ## Advanced
-        
-        ### Hyperlinks for Nested resources
-        
-        **(optional)** If you need hyperlinks for nested relations, you need a custom serializer.
-        
-        There you will inform how to access the *parent* of the instance being serialized when
-        building the *children* URL.
-        
-        In the following example, an instance of Nameserver on `/domain/{domain_pk}/nameservers/{pk}`
-        is being informed that the *parent* Domain should be looked up using the `domain_pk` kwarg
-        from the URL:
-        ```python
-        # serializers.py
-        # (needed only if you want hyperlinks for nested relations on API)
-        from rest_framework_nested.relations import NestedHyperlinkedRelatedField
-        
-        class DomainSerializer(HyperlinkedModelSerializer):
-            class Meta:
-                model = Domain
-        
-            nameservers = HyperlinkedIdentityField(
-                view_name='domain-nameservers-list',
-                lookup_url_kwarg='domain_pk'
-                                # ^-- Nameserver queryset will .get(domain_pk=domain_pk)
-                                #     being this value from URL kwargs
-            )
-        
-        	## OR ##
-        
-            nameservers = NestedHyperlinkedRelatedField(
-                many=True,
-                read_only=True,   # Or add a queryset
-                view_name='domain-nameservers-detail',
-                parent_lookup_kwargs={'domain_pk': 'domain__pk'}
-                                    # ^-- Nameserver queryset will .filter(domain__pk=domain_pk)
-                                    #     being domain_pk (ONE underscore) value from URL kwargs
-            )
-        ```
-        
-        **(optional)** If you want a little bit more control over the fields displayed for the nested relations while looking at the parent, you need a custom serializer using NestedHyperlinkedModelSerializer.
-        ```python
-        from rest_framework.serializers import HyperlinkedModelSerializer
-        from rest_framework_nested.serializers import NestedHyperlinkedModelSerializer
-        
-        class NameserverSerializers(HyperlinkedModelSerializer):
-        	class Meta:
-        		model = Nameserver
-        		fields = (...)
-        
-        
-        class DomainNameserverSerializers(NestedHyperlinkedModelSerializer):
-        	parent_lookup_kwargs = {
-        		'domain_pk': 'domain__pk',
-        	}
-        	class Meta:
-        		model = Nameserver
-        		fields = ('url', ...)
-        
-        
-        class DomainSerializer(HyperlinkedModelSerializer):
-        	class Meta:
-        		model = Domain
-        		fields = (..., 'nameservers')
-        
-        	nameservers = DomainNameserverSerializers(many=True, read_only=True)
-        ```
-        
-        ### Infinite-depth Nesting
-        
-        Example of nested router 3 levels deep.
-        You can use this same logic to nest routers as deep as you need.
-        This example ahead accomplishes the below URL patterns.
-        ```
-        /clients/
-        /clients/{pk}/
-        /clients/{client_pk}/maildrops/
-        /clients/{client_pk}/maildrops/{pk}/
-        /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/
-        /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/{pk}/
-        ```
-        
-        ```python
-        # urls.py
-        router = DefaultRouter()
-        router.register(r'clients', ClientViewSet, basename='clients')
-        ## generates:
-        # /clients/
-        # /clients/{pk}/
-        
-        client_router = routers.NestedSimpleRouter(router, r'clients', lookup='client')
-        client_router.register(r'maildrops', MailDropViewSet, basename='maildrops')
-        ## generates:
-        # /clients/{client_pk}/maildrops/
-        # /clients/{client_pk}/maildrops/{pk}/
-        
-        maildrops_router = routers.NestedSimpleRouter(client_router, r'maildrops', lookup='maildrop')
-        maildrops_router.register(r'recipients', MailRecipientViewSet, basename='recipients')
-        ## generates:
-        # /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/
-        # /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/{pk}/
-        
-        urlpatterns = [
-            path(r'', include(router.urls)),
-            path(r'', include(client_router.urls)),
-            path(r'', include(maildrops_router.urls)),
-        ]
-        ```
-        
-        ```python
-        # views.py
-        class ClientViewSet(viewsets.ViewSet):
-            serializer_class = ClientSerializer
-        
-            def list(self, request,):
-                queryset = Client.objects.filter()
-                serializer = ClientSerializer(queryset, many=True)
-                return Response(serializer.data)
-        
-            def retrieve(self, request, pk=None):
-                queryset = Client.objects.filter()
-                client = get_object_or_404(queryset, pk=pk)
-                serializer = ClientSerializer(client)
-                return Response(serializer.data)
-        
-        
-        class MailDropViewSet(viewsets.ViewSet):
-            serializer_class = MailDropSerializer
-        
-            def list(self, request, client_pk=None):
-                queryset = MailDrop.objects.filter(client=client_pk)
-                serializer = MailDropSerializer(queryset, many=True)
-                return Response(serializer.data)
-        
-            def retrieve(self, request, pk=None, client_pk=None):
-                queryset = MailDrop.objects.filter(pk=pk, client=client_pk)
-                maildrop = get_object_or_404(queryset, pk=pk)
-                serializer = MailDropSerializer(maildrop)
-                return Response(serializer.data)
-        
-        
-        class MailRecipientViewSet(viewsets.ViewSet):
-            serializer_class = MailRecipientSerializer
-        
-            def list(self, request, client_pk=None, maildrop_pk=None):
-                queryset = MailRecipient.objects.filter(mail_drop__client=client_pk, mail_drop=maildrop_pk)
-                serializer = MailRecipientSerializer(queryset, many=True)
-                return Response(serializer.data)
-        
-            def retrieve(self, request, pk=None, client_pk=None, maildrop_pk=None):
-                queryset = MailRecipient.objects.filter(pk=pk, mail_drop=maildrop_pk, mail_drop__client=client_pk)
-                maildrop = get_object_or_404(queryset, pk=pk)
-                serializer = MailRecipientSerializer(maildrop)
-                return Response(serializer.data)
-        ```
-        
-        ```python
-        # serializers.py
-        class ClientSerializer(HyperlinkedModelSerializer):
-            class Meta:
-                model = Client
-                fields = (...)
-        
-        
-        class MailDropSerializer(NestedHyperlinkedModelSerializer):
-            parent_lookup_kwargs = {
-                'client_pk': 'client__pk',
-            }
-            class Meta:
-                model = MailDrop
-                fields = (...)
-        
-        
-        class MailRecipientSerializer(NestedHyperlinkedModelSerializer):
-            parent_lookup_kwargs = {
-                'maildrop_pk': 'mail_drop__pk',
-                'client_pk': 'mail_drop__client__pk',
-            }
-            class Meta:
-                model = MailRecipient
-                fields = (...)
-        ```
-        
-        ## Testing
-        
-        In order to get started with testing, you will need to install [tox](https://tox.readthedocs.io/en/latest/).
-        Once installed, you can then run one environment locally, to speed up your development cycle:
-        
-        ```
-        $ tox -e py39-django3.1-drf3.11
-        ```
-        
-        Once you submit a pull request, your changes will be run against many environments with GitHub Actions named CI.
-        
-        
-        ## License
-        
-        This package is licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-        and can undestand more at http://choosealicense.com/licenses/apache/ on the
-        sidebar notes.
-        
-        Apache Licence v2.0 is a MIT-like licence. This means, in plain English:
-        - It's truly open source
-        - You can use it as you wish, for money or not
-        - You can sublicence it (change the licence!!)
-        - This way, you can even use it on your closed-source project
-        As long as:
-        - You cannot use the authors name, logos, etc, to endorse a project
-        - You keep the authors copyright notices where this code got used, even on your closed-source project
-        (come on, even Microsoft kept BSD notices on Windows about its TCP/IP stack :P)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
@@ -324,7 +20,311 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+**This is a work in progress. It "works for me" at www.apiregistro.com.br,
+but I cannot warranty that it fully "works everywhere" yet. Join us on Gitter (below) if you need some help.**
+
+# drf-nested-routers
+
+[![Join the chat at https://gitter.im/alanjds/drf-nested-routers](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/alanjds/drf-nested-routers?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Build Status](https://github.com/alanjds/drf-nested-routers/workflows/CI/badge.svg)](https://github.com/alanjds/drf-nested-routers/actions?query=workflow%3ACI+branch%3Amaster)
+
+This package provides routers and fields to create nested resources in the [Django Rest Framework](http://django-rest-framework.org/)
+
+Nested resources are needed for full REST URL structure, if one resource lives inside another.
+
+The following example is about Domains and DNS Nameservers.
+There are many domains, and each domain has many nameservers. The "nameserver" resource does not
+exist without a domain, so you need it "nested" inside the domain.
+
+
+## Requirements & Compatibility
+
+-  Python (3.8, 3.9, 3.10, 3.11)
+-  Django (3.2, 4.1, 4.2)
+-  Django REST Framework (3.14)
+
+It may work with lower versions, but since the release **0.93.5** is no more tested on CI for Python 3.6 or lower.<br/>
+And since **0.92.1** is no more tested on CI for Pythons 2.7 to 3.5, Django 1.11 to 2.1 or DRF 3.6 to 3.10.<br/>
+Before that, the release **0.90.2** was tested also with DRF 2.4.3 up to 3.7.
+
+
+## Installation
+
+You can install this library using pip:
+
+```pip install drf-nested-routers```
+
+It is not needed to add this library in your Django project's `settings.py` file, as it does not contain any app, signal or model.
+
+## Quickstart
+
+The desired URL signatures are:
+```
+/domains/ <- Domains list
+/domains/{pk}/ <- One domain, from {pk}
+/domains/{domain_pk}/nameservers/ <- Nameservers of domain from {domain_pk}
+/domains/{domain_pk}/nameservers/{pk} <- Specific nameserver from {pk}, of domain from {domain_pk}
+```
+
+How to do it (example):
+```python
+# urls.py
+from rest_framework_nested import routers
+from views import DomainViewSet, NameserverViewSet
+(...)
+
+router = routers.SimpleRouter()
+router.register(r'domains', DomainViewSet)
+
+domains_router = routers.NestedSimpleRouter(router, r'domains', lookup='domain')
+domains_router.register(r'nameservers', NameserverViewSet, basename='domain-nameservers')
+# 'basename' is optional. Needed only if the same viewset is registered more than once
+# Official DRF docs on this option: http://www.django-rest-framework.org/api-guide/routers/
+
+urlpatterns = [
+    path(r'', include(router.urls)),
+    path(r'', include(domains_router.urls)),
+]
+```
+
+```python
+# views.py
+
+## For Django' ORM-based resources ##
+
+class NameserverViewSet(viewsets.ModelViewSet):
+    def get_queryset(self):
+        return Nameserver.objects.filter(domain=self.kwargs['domain_pk'])
+
+## OR: non-ORM resources ##
+
+class NameserverViewSet(viewsets.ViewSet):
+    def list(self, request, domain_pk=None):
+        nameservers = self.queryset.filter(domain=domain_pk)
+        (...)
+        return Response([...])
+
+    def retrieve(self, request, pk=None, domain_pk=None):
+        nameservers = self.queryset.get(pk=pk, domain=domain_pk)
+        (...)
+        return Response(serializer.data)
+```
+
+## Advanced
+
+### Hyperlinks for Nested resources
+
+**(optional)** If you need hyperlinks for nested relations, you need a custom serializer.
+
+There you will inform how to access the *parent* of the instance being serialized when
+building the *children* URL.
+
+In the following example, an instance of Nameserver on `/domain/{domain_pk}/nameservers/{pk}`
+is being informed that the *parent* Domain should be looked up using the `domain_pk` kwarg
+from the URL:
+```python
+# serializers.py
+# (needed only if you want hyperlinks for nested relations on API)
+from rest_framework_nested.relations import NestedHyperlinkedRelatedField
+
+class DomainSerializer(HyperlinkedModelSerializer):
+    class Meta:
+        model = Domain
+
+    nameservers = HyperlinkedIdentityField(
+        view_name='domain-nameservers-list',
+        lookup_url_kwarg='domain_pk'
+                        # ^-- Nameserver queryset will .get(domain_pk=domain_pk)
+                        #     being this value from URL kwargs
+    )
+
+	## OR ##
+
+    nameservers = NestedHyperlinkedRelatedField(
+        many=True,
+        read_only=True,   # Or add a queryset
+        view_name='domain-nameservers-detail',
+        parent_lookup_kwargs={'domain_pk': 'domain__pk'}
+                            # ^-- Nameserver queryset will .filter(domain__pk=domain_pk)
+                            #     being domain_pk (ONE underscore) value from URL kwargs
+    )
+```
+
+**(optional)** If you want a little bit more control over the fields displayed for the nested relations while looking at the parent, you need a custom serializer using NestedHyperlinkedModelSerializer.
+```python
+from rest_framework.serializers import HyperlinkedModelSerializer
+from rest_framework_nested.serializers import NestedHyperlinkedModelSerializer
+
+class NameserverSerializers(HyperlinkedModelSerializer):
+	class Meta:
+		model = Nameserver
+		fields = (...)
+
+
+class DomainNameserverSerializers(NestedHyperlinkedModelSerializer):
+	parent_lookup_kwargs = {
+		'domain_pk': 'domain__pk',
+	}
+	class Meta:
+		model = Nameserver
+		fields = ('url', ...)
+
+
+class DomainSerializer(HyperlinkedModelSerializer):
+	class Meta:
+		model = Domain
+		fields = (..., 'nameservers')
+
+	nameservers = DomainNameserverSerializers(many=True, read_only=True)
+```
+
+### Infinite-depth Nesting
+
+Example of nested router 3 levels deep.
+You can use this same logic to nest routers as deep as you need.
+This example ahead accomplishes the below URL patterns.
+```
+/clients/
+/clients/{pk}/
+/clients/{client_pk}/maildrops/
+/clients/{client_pk}/maildrops/{pk}/
+/clients/{client_pk}/maildrops/{maildrop_pk}/recipients/
+/clients/{client_pk}/maildrops/{maildrop_pk}/recipients/{pk}/
+```
+
+```python
+# urls.py
+router = DefaultRouter()
+router.register(r'clients', ClientViewSet, basename='clients')
+## generates:
+# /clients/
+# /clients/{pk}/
+
+client_router = routers.NestedSimpleRouter(router, r'clients', lookup='client')
+client_router.register(r'maildrops', MailDropViewSet, basename='maildrops')
+## generates:
+# /clients/{client_pk}/maildrops/
+# /clients/{client_pk}/maildrops/{pk}/
+
+maildrops_router = routers.NestedSimpleRouter(client_router, r'maildrops', lookup='maildrop')
+maildrops_router.register(r'recipients', MailRecipientViewSet, basename='recipients')
+## generates:
+# /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/
+# /clients/{client_pk}/maildrops/{maildrop_pk}/recipients/{pk}/
+
+urlpatterns = [
+    path(r'', include(router.urls)),
+    path(r'', include(client_router.urls)),
+    path(r'', include(maildrops_router.urls)),
+]
+```
+
+```python
+# views.py
+class ClientViewSet(viewsets.ViewSet):
+    serializer_class = ClientSerializer
+
+    def list(self, request,):
+        queryset = Client.objects.filter()
+        serializer = ClientSerializer(queryset, many=True)
+        return Response(serializer.data)
+
+    def retrieve(self, request, pk=None):
+        queryset = Client.objects.filter()
+        client = get_object_or_404(queryset, pk=pk)
+        serializer = ClientSerializer(client)
+        return Response(serializer.data)
+
+
+class MailDropViewSet(viewsets.ViewSet):
+    serializer_class = MailDropSerializer
+
+    def list(self, request, client_pk=None):
+        queryset = MailDrop.objects.filter(client=client_pk)
+        serializer = MailDropSerializer(queryset, many=True)
+        return Response(serializer.data)
+
+    def retrieve(self, request, pk=None, client_pk=None):
+        queryset = MailDrop.objects.filter(pk=pk, client=client_pk)
+        maildrop = get_object_or_404(queryset, pk=pk)
+        serializer = MailDropSerializer(maildrop)
+        return Response(serializer.data)
+
+
+class MailRecipientViewSet(viewsets.ViewSet):
+    serializer_class = MailRecipientSerializer
+
+    def list(self, request, client_pk=None, maildrop_pk=None):
+        queryset = MailRecipient.objects.filter(mail_drop__client=client_pk, mail_drop=maildrop_pk)
+        serializer = MailRecipientSerializer(queryset, many=True)
+        return Response(serializer.data)
+
+    def retrieve(self, request, pk=None, client_pk=None, maildrop_pk=None):
+        queryset = MailRecipient.objects.filter(pk=pk, mail_drop=maildrop_pk, mail_drop__client=client_pk)
+        maildrop = get_object_or_404(queryset, pk=pk)
+        serializer = MailRecipientSerializer(maildrop)
+        return Response(serializer.data)
+```
+
+```python
+# serializers.py
+class ClientSerializer(HyperlinkedModelSerializer):
+    class Meta:
+        model = Client
+        fields = (...)
+
+
+class MailDropSerializer(NestedHyperlinkedModelSerializer):
+    parent_lookup_kwargs = {
+        'client_pk': 'client__pk',
+    }
+    class Meta:
+        model = MailDrop
+        fields = (...)
+
+
+class MailRecipientSerializer(NestedHyperlinkedModelSerializer):
+    parent_lookup_kwargs = {
+        'maildrop_pk': 'mail_drop__pk',
+        'client_pk': 'mail_drop__client__pk',
+    }
+    class Meta:
+        model = MailRecipient
+        fields = (...)
+```
+
+## Testing
+
+In order to get started with testing, you will need to install [tox](https://tox.readthedocs.io/en/latest/).
+Once installed, you can then run one environment locally, to speed up your development cycle:
+
+```
+$ tox -e py39-django3.1-drf3.11
+```
+
+Once you submit a pull request, your changes will be run against many environments with GitHub Actions named CI.
+
+
+## License
+
+This package is licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+and can undestand more at http://choosealicense.com/licenses/apache/ on the
+sidebar notes.
+
+Apache Licence v2.0 is a MIT-like licence. This means, in plain English:
+- It's truly open source
+- You can use it as you wish, for money or not
+- You can sublicence it (change the licence!!)
+- This way, you can even use it on your closed-source project
+As long as:
+- You cannot use the authors name, logos, etc, to endorse a project
+- You keep the authors copyright notices where this code got used, even on your closed-source project
+(come on, even Microsoft kept BSD notices on Windows about its TCP/IP stack :P)
```

### Comparing `drf-nested-routers-0.93.5/drf_nested_routers.egg-info/SOURCES.txt` & `drf-nested-routers-0.94.0/drf_nested_routers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-README.rst
 requirements.txt
 setup.cfg
 setup.py
 drf_nested_routers.egg-info/PKG-INFO
 drf_nested_routers.egg-info/SOURCES.txt
 drf_nested_routers.egg-info/dependency_links.txt
 drf_nested_routers.egg-info/requires.txt
```

### Comparing `drf-nested-routers-0.93.5/rest_framework_nested/__init__.py` & `drf-nested-routers-0.94.0/rest_framework_nested/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '0.93.5'
+__version__ = '0.94.0'
```

### Comparing `drf-nested-routers-0.93.5/rest_framework_nested/relations.py` & `drf-nested-routers-0.94.0/rest_framework_nested/relations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """
 Serializer fields that deal with relationships with nested resources.
 
 These fields allow you to specify the style that should be used to represent
 model relationships with hyperlinks.
 """
-from __future__ import unicode_literals
-from functools import reduce  # import reduce from functools for compatibility with python 3
+from __future__ import annotations
 
-import rest_framework.relations
-from rest_framework.relations import ObjectDoesNotExist, ObjectValueError, ObjectTypeError
+from functools import reduce
+from typing import Any, Generic, TypeVar
+
+from django.core.exceptions import ObjectDoesNotExist
+from django.db.models import Model
+from rest_framework.relations import HyperlinkedRelatedField, ObjectTypeError, ObjectValueError
 from rest_framework.exceptions import ValidationError
+from rest_framework.request import Request
+
 
-# fix for basestring
-try:
-    basestring
-except NameError:
-    basestring = str
+T_Model = TypeVar('T_Model', bound=Model)
 
 
-class NestedHyperlinkedRelatedField(rest_framework.relations.HyperlinkedRelatedField):
+class NestedHyperlinkedRelatedField(HyperlinkedRelatedField, Generic[T_Model]):
     lookup_field = 'pk'
     parent_lookup_kwargs = {
         'parent_pk': 'parent__pk'
     }
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         self.parent_lookup_kwargs = kwargs.pop('parent_lookup_kwargs', self.parent_lookup_kwargs)
-        super(NestedHyperlinkedRelatedField, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
-    def get_url(self, obj, view_name, request, format):
+    def get_url(self, obj: Model, view_name: str, request: Request, format: str | None) -> str | None:
         """
         Given an object, return the URL that hyperlinks to the object.
 
         May raise a `NoReverseMatch` if the `view_name` and `lookup_field`
         attributes are not configured to correctly match the URL conf.
         """
         # Unsaved objects will not yet have a valid URL.
@@ -49,25 +50,25 @@
 
             # split each lookup by their __, e.g. "parent__pk" will be split into "parent" and "pk", or
             # "parent__super__pk" would be split into "parent", "super" and "pk"
             lookups = underscored_lookup.split('__')
 
             try:
                 # use the Django ORM to lookup this value, e.g., obj.parent.pk
-                lookup_value = reduce(getattr, [obj] + lookups)
+                lookup_value = reduce(getattr, [obj] + lookups)  # type: ignore[operator,arg-type]
             except AttributeError:
                 # Not nested. Act like a standard HyperlinkedRelatedField
                 return super().get_url(obj, view_name, request, format)
 
             # store the lookup_name and value in kwargs, which is later passed to the reverse method
             kwargs.update({parent_lookup_kwarg: lookup_value})
 
         return self.reverse(view_name, kwargs=kwargs, request=request, format=format)
 
-    def get_object(self, view_name, view_args, view_kwargs):
+    def get_object(self, view_name: str, view_args: list[Any], view_kwargs: dict[str, Any]) -> T_Model:
         """
         Return the object corresponding to a matched URL.
 
         Takes the matched URL conf arguments, and should return an
         object instance, or raise an `ObjectDoesNotExist` exception.
         """
         # default lookup from rest_framework.relations.HyperlinkedRelatedField
@@ -77,30 +78,30 @@
         # multi-level lookup
         for parent_lookup_kwarg in list(self.parent_lookup_kwargs.keys()):
             lookup_value = view_kwargs[parent_lookup_kwarg]
             kwargs.update({self.parent_lookup_kwargs[parent_lookup_kwarg]: lookup_value})
 
         return self.get_queryset().get(**kwargs)
 
-    def use_pk_only_optimization(self):
+    def use_pk_only_optimization(self) -> bool:
         return False
 
-    def to_internal_value(self, data):
+    def to_internal_value(self, data: Any) -> T_Model:
         try:
             return super().to_internal_value(data)
         except ValidationError as err:
-            if err.detail[0].code != 'no_match':
+            if err.detail[0].code != 'no_match':  # type: ignore[union-attr,index]
                 raise
 
             # data is probable the lookup value, not the resource URL
             try:
                 return self.get_queryset().get(**{self.lookup_field: data})
             except (ObjectDoesNotExist, ObjectValueError, ObjectTypeError):
                 self.fail('does_not_exist')
 
 
-class NestedHyperlinkedIdentityField(NestedHyperlinkedRelatedField):
-    def __init__(self, view_name=None, **kwargs):
+class NestedHyperlinkedIdentityField(NestedHyperlinkedRelatedField[T_Model]):
+    def __init__(self, view_name: str | None = None, **kwargs: Any) -> None:
         assert view_name is not None, 'The `view_name` argument is required.'
         kwargs['read_only'] = True
         kwargs['source'] = '*'
-        super(NestedHyperlinkedIdentityField, self).__init__(view_name=view_name, **kwargs)
+        super().__init__(view_name=view_name, **kwargs)
```

### Comparing `drf-nested-routers-0.93.5/rest_framework_nested/routers.py` & `drf-nested-routers-0.94.0/rest_framework_nested/routers.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,42 +21,50 @@
     router = routers.DefaultRouter()
     router.register('users', UserViewSet, 'user')
     router.register('accounts', AccountViewSet, 'account')
 
     urlpatterns = router.urls
 """
 
-from __future__ import unicode_literals
+from __future__ import annotations
+
 import sys
 import re
-from rest_framework.routers import SimpleRouter, DefaultRouter  # noqa: F401
+from typing import Any
 
+from rest_framework.routers import DefaultRouter, SimpleRouter
 
 if sys.version_info[0] < 3:
     IDENTIFIER_REGEX = re.compile(r"^[^\d\W]\w*$")
 else:
     IDENTIFIER_REGEX = re.compile(r"^[^\d\W]\w*$", re.UNICODE)
 
 
-class LookupMixin(object):
+class LookupMixin:
     """
     Deprecated.
 
     No method override is needed since Django Rest Framework 2.4.
     """
 
 
-class NestedMixin(object):
-    def __init__(self, parent_router, parent_prefix, *args, **kwargs):
+class NestedMixin:
+    def __init__(
+        self,
+        parent_router: SimpleRouter | DefaultRouter | NestedMixin,
+        parent_prefix: str,
+        *args: Any,
+        **kwargs: Any
+    ) -> None:
         self.parent_router = parent_router
         self.parent_prefix = parent_prefix
         self.nest_count = getattr(parent_router, 'nest_count', 0) + 1
-        self.nest_prefix = kwargs.pop('lookup', 'nested_%i' % self.nest_count) + '_'
+        self.nest_prefix = kwargs.pop('lookup', f'nested_{self.nest_count}') + '_'
 
-        super(NestedMixin, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         if 'trailing_slash' not in kwargs:
             # Inherit trailing_slash only when not specified explicitly.
             #
             # drf transposes the trailing_slash argument into the actual appended value
             # within the route urls. This means that, on the parent class, trailing_slash
             # is either '/' or '' for the expected kwarg values True or False, respectively.
@@ -64,61 +72,60 @@
             # those two values (for example, to add an optional slash with '/?'), we won't
             # be able to set it through the kwargs.
             #
             # By copying the value of trailing_slash directly, we ensure that our inherited
             # behavior is ALWAYS consistent with the parent. If we didn't, we might create
             # a situation where the parent's trailing slash is truthy (but not '/') and
             # we set our trailing slash to just '/', leading to inconsistent behavior.
-            self.trailing_slash = parent_router.trailing_slash
+            self.trailing_slash = parent_router.trailing_slash  # type: ignore[has-type]
 
-        parent_registry = [registered for registered
-                           in self.parent_router.registry
-                           if registered[0] == self.parent_prefix]
+        parent_registry = [
+            registered for registered
+            in self.parent_router.registry  # type: ignore[union-attr]
+            if registered[0] == self.parent_prefix
+        ]
         try:
-            parent_registry = parent_registry[0]
-            parent_prefix, parent_viewset, parent_basename = parent_registry
+            parent_registry_item = parent_registry[0]
+            parent_prefix, parent_viewset, parent_basename = parent_registry_item
         except:
             raise RuntimeError('parent registered resource not found')
 
         self.check_valid_name(self.nest_prefix)
 
         nested_routes = []
-        parent_lookup_regex = parent_router.get_lookup_regex(parent_viewset, self.nest_prefix)
+        parent_lookup_regex = parent_router.get_lookup_regex(parent_viewset, self.nest_prefix)  # type: ignore[union-attr]
 
-        self.parent_regex = '{parent_prefix}/{parent_lookup_regex}/'.format(
-            parent_prefix=parent_prefix,
-            parent_lookup_regex=parent_lookup_regex
-        )
+        self.parent_regex = f'{parent_prefix}/{parent_lookup_regex}/'
         # If there is no parent prefix, the first part of the url is probably
         #   controlled by the project's urls.py and the router is in an app,
         #   so a slash in the beginning will (A) cause Django to give warnings
         #   and (B) generate URLs that will require using `//`
         if not self.parent_prefix and self.parent_regex[0] == '/':
             self.parent_regex = self.parent_regex[1:]
         if hasattr(parent_router, 'parent_regex'):
             self.parent_regex = parent_router.parent_regex + self.parent_regex
 
-        for route in self.routes:
+        for route in self.routes:  # type: ignore[has-type]
             route_contents = route._asdict()
 
             # This will get passed through .format in a little bit, so we need
             # to escape it
             escaped_parent_regex = self.parent_regex.replace('{', '{{').replace('}', '}}')
 
             route_contents['url'] = route.url.replace('^', '^' + escaped_parent_regex)
             nested_routes.append(type(route)(**route_contents))
 
         self.routes = nested_routes
 
-    def check_valid_name(self, value):
+    def check_valid_name(self, value: str) -> None:
         if IDENTIFIER_REGEX.match(value) is None:
-            raise ValueError("lookup argument '{}' needs to be valid python identifier".format(value))
+            raise ValueError(f"lookup argument '{value}' needs to be valid python identifier")
 
 
-class NestedSimpleRouter(NestedMixin, SimpleRouter):
+class NestedSimpleRouter(NestedMixin, SimpleRouter):  # type: ignore[misc]
     """ Create a NestedSimpleRouter nested within `parent_router`
     Args:
 
     parent_router: Parent router. Maybe be a SimpleRouter or another nested
         router.
 
     parent_prefix: The url prefix within parent_router under which the
@@ -131,15 +138,15 @@
         on 'pk' so the parent lookup regex will be 'domain_pk'.
         Default: 'nested_<n>' where <n> is 1+parent_router.nest_count
 
     """
     pass
 
 
-class NestedDefaultRouter(NestedMixin, DefaultRouter):
+class NestedDefaultRouter(NestedMixin, DefaultRouter):  # type: ignore[misc]
     """ Create a NestedDefaultRouter nested within `parent_router`
     Args:
 
     parent_router: Parent router. Maybe be a DefaultRouter or another nested
         router.
 
     parent_prefix: The url prefix within parent_router under which the
```

### Comparing `drf-nested-routers-0.93.5/rest_framework_nested/runtests/runcoverage.py` & `drf-nested-routers-0.94.0/rest_framework_nested/runtests/runcoverage.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,41 +4,43 @@
 """
 
 # http://ericholscher.com/blog/2009/jun/29/enable-setuppy-test-your-django-apps/
 # http://www.travisswicegood.com/2010/01/17/django-virtualenv-pip-and-fabric/
 # http://code.djangoproject.com/svn/django/trunk/tests/runtests.py
 import os
 import sys
+from typing import NoReturn
 from coverage import coverage
 
 # fix sys path so we don't need to setup PYTHONPATH
 sys.path.append(os.path.join(os.path.dirname(__file__), "../.."))
 os.environ['DJANGO_SETTINGS_MODULE'] = 'rest_framework_nested.runtests.settings'
 
 
-def main():
+def main() -> NoReturn:
     """Run the tests for rest_framework and generate a coverage report."""
 
     cov = coverage()
     cov.erase()
     cov.start()
 
     from django.conf import settings
     from django.test.utils import get_runner
     TestRunner = get_runner(settings)
 
+    failures: int
     if hasattr(TestRunner, 'func_name'):
         # Pre 1.2 test runners were just functions,
         # and did not support the 'failfast' option.
         import warnings
         warnings.warn(
             'Function-based test runners are deprecated. Test runners should be classes with a run_tests() method.',
             DeprecationWarning
         )
-        failures = TestRunner(['tests'])
+        failures = TestRunner(['tests'])  # type: ignore[assignment,arg-type]
     else:
         test_runner = TestRunner()
         failures = test_runner.run_tests(['tests'])
     cov.stop()
 
     # Discover the list of all modules that we should test coverage for
     import rest_framework
```

### Comparing `drf-nested-routers-0.93.5/rest_framework_nested/runtests/runtests.py` & `drf-nested-routers-0.94.0/rest_framework_nested/runtests/runtests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 #!/usr/bin/env python
 
 # http://ericholscher.com/blog/2009/jun/29/enable-setuppy-test-your-django-apps/
 # http://www.travisswicegood.com/2010/01/17/django-virtualenv-pip-and-fabric/
 # http://code.djangoproject.com/svn/django/trunk/tests/runtests.py
 import os
 import sys
+from typing import NoReturn
 
 # fix sys path so we don't need to setup PYTHONPATH
 sys.path.append(os.path.join(os.path.dirname(__file__), "../.."))
 os.environ['DJANGO_SETTINGS_MODULE'] = 'rest_framework_nested.runtests.settings'
 
 import django
 from django.conf import settings
 from django.test.utils import get_runner
 
 
-def usage():
+def usage() -> str:
     return """
     Usage: python runtests.py [UnitTestClass].[method]
 
     You can pass the Class name of the `UnitTestClass` you want to test.
 
     Append a method name if you only want to test a specific method of that class.
     """
 
 
-def main():
+def main() -> NoReturn:
     TestRunner = get_runner(settings)
     import ipdb
     ipdb.set_trace()
 
     test_runner = TestRunner()
     if len(sys.argv) == 2:
         test_case = '.' + sys.argv[1]
```

### Comparing `drf-nested-routers-0.93.5/rest_framework_nested/runtests/settings.py` & `drf-nested-routers-0.94.0/rest_framework_nested/runtests/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 # Django settings for testproject project.
 
 DEBUG = True
 TEMPLATE_DEBUG = DEBUG
 DEBUG_PROPAGATE_EXCEPTIONS = True
 
 ALLOWED_HOSTS = ['*']
@@ -79,64 +81,64 @@
 
 TEMPLATE_DIRS = (
     # Put strings here, like "/home/html/django_templates" or "C:/www/django/templates".
     # Always use forward slashes, even on Windows.
     # Don't forget to use absolute paths, not relative paths.
 )
 
-INSTALLED_APPS = (
+INSTALLED_APPS = [
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.sites',
     'django.contrib.messages',
     # Uncomment the next line to enable the admin:
     # 'django.contrib.admin',
     # Uncomment the next line to enable admin documentation:
     # 'django.contrib.admindocs',
     # 'rest_framework.authtoken',
     'rest_framework_nested',
     'rest_framework_nested.tests',
-)
+]
 
 # OAuth is optional and won't work if there is no oauth_provider & oauth2
 try:
     import oauth_provider  # noqa: F401
     import oauth2  # noqa: F401
 except ImportError:
     pass
 else:
-    INSTALLED_APPS += (
+    INSTALLED_APPS += [
         'oauth_provider',
-    )
+    ]
 
 try:
     import provider  # noqa: F401
 except ImportError:
     pass
 else:
-    INSTALLED_APPS += (
+    INSTALLED_APPS += [
         'provider',
         'provider.oauth2',
-    )
+    ]
 
 # guardian is optional
 try:
     import guardian  # noqa: F401
 except ImportError:
     pass
 else:
     ANONYMOUS_USER_ID = -1
     AUTHENTICATION_BACKENDS = (
         'django.contrib.auth.backends.ModelBackend',  # default
         'guardian.backends.ObjectPermissionBackend',
     )
-    INSTALLED_APPS += (
+    INSTALLED_APPS += [
         'guardian',
-    )
+    ]
 
 STATIC_URL = '/static/'
 
 PASSWORD_HASHERS = (
     'django.contrib.auth.hashers.SHA1PasswordHasher',
     'django.contrib.auth.hashers.PBKDF2PasswordHasher',
     'django.contrib.auth.hashers.PBKDF2SHA1PasswordHasher',
```

### Comparing `drf-nested-routers-0.93.5/rest_framework_nested/serializers.py` & `drf-nested-routers-0.94.0/rest_framework_nested/serializers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+from __future__ import annotations
+
+from typing import Any, TypeVar
+
 import rest_framework.serializers
+from django.db.models import Model
+from rest_framework.fields import Field
+from rest_framework.utils.model_meta import RelationInfo
 from rest_framework_nested.relations import NestedHyperlinkedIdentityField, NestedHyperlinkedRelatedField
 try:
     from rest_framework.utils.field_mapping import get_nested_relation_kwargs
 except ImportError:
     pass
     # passing because NestedHyperlinkedModelSerializer can't be used anyway
     #    if version too old.
 
 
-class NestedHyperlinkedModelSerializer(rest_framework.serializers.HyperlinkedModelSerializer):
+T_Model = TypeVar('T_Model', bound=Model)
+
+
+class NestedHyperlinkedModelSerializer(rest_framework.serializers.HyperlinkedModelSerializer[T_Model]):
     """
     A type of `ModelSerializer` that uses hyperlinked relationships with compound keys instead
     of primary key relationships.  Specifically:
 
     * A 'url' field is included instead of the 'id' field.
     * Relationships to other instances are hyperlinks, instead of primary keys.
 
@@ -21,28 +31,30 @@
     parent_lookup_kwargs = {
         'parent_pk': 'parent__pk'
     }
 
     serializer_url_field = NestedHyperlinkedIdentityField
     serializer_related_field = NestedHyperlinkedRelatedField
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         self.parent_lookup_kwargs = kwargs.pop('parent_lookup_kwargs', self.parent_lookup_kwargs)
-        super(NestedHyperlinkedModelSerializer, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
-    def build_url_field(self, field_name, model_class):
-        field_class, field_kwargs = super(NestedHyperlinkedModelSerializer, self).build_url_field(
+    def build_url_field(self, field_name: str, model_class: T_Model) -> tuple[type[Field], dict[str, Any]]:
+        field_class, field_kwargs = super().build_url_field(
             field_name,
             model_class
         )
         field_kwargs['parent_lookup_kwargs'] = self.parent_lookup_kwargs
 
         return field_class, field_kwargs
 
-    def build_nested_field(self, field_name, relation_info, nested_depth):
+    def build_nested_field(
+        self, field_name: str, relation_info: RelationInfo, nested_depth: int
+    ) -> tuple[type[Field], dict[str, Any]]:
         """
         Create nested fields for forward and reverse relationships.
         """
         class NestedSerializer(NestedHyperlinkedModelSerializer):
             class Meta:
                 model = relation_info.related_model
                 depth = nested_depth - 1
```

### Comparing `drf-nested-routers-0.93.5/rest_framework_nested/viewsets.py` & `drf-nested-routers-0.94.0/rest_framework_nested/viewsets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,82 @@
+from __future__ import annotations
+
 import contextlib
+from typing import Any, Generic, Iterator, TypeVar
 
 from django.core.exceptions import ImproperlyConfigured
+from django.db.models import Model, QuerySet
+from django.http import HttpRequest, QueryDict
+from rest_framework.request import Request
+from rest_framework.serializers import BaseSerializer
+
+T_Model = TypeVar('T_Model', bound=Model)
 
 
 @contextlib.contextmanager
-def _force_mutable(querydict: dict) -> dict:
+def _force_mutable(querydict: QueryDict | dict[str, Any]) -> Iterator[QueryDict | dict[str, Any]]:
     """
     Takes a HttpRequest querydict from Django and forces it to be mutable.
     Reverts the initial state back on exit, if any.
     """
     initial_mutability = getattr(querydict, '_mutable', None)
     if initial_mutability is not None:
-        querydict._mutable = True
+        querydict._mutable = True  # type: ignore[union-attr]
     yield querydict
     if initial_mutability is not None:
-        querydict._mutable = initial_mutability
+        querydict._mutable = initial_mutability  # type: ignore[union-attr]
 
 
-class NestedViewSetMixin(object):
-    def _get_parent_lookup_kwargs(self) -> dict:
+class NestedViewSetMixin(Generic[T_Model]):
+    def _get_parent_lookup_kwargs(self) -> dict[str, str]:
         """
         Locates and returns the `parent_lookup_kwargs` dict informing
         how the kwargs in the URL maps to the parents of the model instance
 
         For now, fetches from `parent_lookup_kwargs`
         on the ViewSet or Serializer attached. This may change on the future.
         """
         parent_lookup_kwargs = getattr(self, 'parent_lookup_kwargs', None)
 
         if not parent_lookup_kwargs:
-            serializer_class = self.get_serializer_class()
+            serializer_class: type[BaseSerializer[T_Model]] = self.get_serializer_class()  # type: ignore[attr-defined]
             parent_lookup_kwargs = getattr(serializer_class, 'parent_lookup_kwargs', None)
 
         if not parent_lookup_kwargs:
             raise ImproperlyConfigured(
                 "NestedViewSetMixin need 'parent_lookup_kwargs' to find the parent from the URL"
             )
 
         return parent_lookup_kwargs
 
-    def get_queryset(self):
+    def get_queryset(self) -> QuerySet[T_Model]:
         """
         Filter the `QuerySet` based on its parents as defined in the
         `serializer_class.parent_lookup_kwargs` or `viewset.parent_lookup_kwargs`
         """
-        queryset = super(NestedViewSetMixin, self).get_queryset()
+        queryset = super().get_queryset()  # type: ignore[misc]
 
         if getattr(self, 'swagger_fake_view', False):
             return queryset
 
-        orm_filters = {}
+        orm_filters: dict[str, Any] = {}
         parent_lookup_kwargs = self._get_parent_lookup_kwargs()
         for query_param, field_name in parent_lookup_kwargs.items():
-            orm_filters[field_name] = self.kwargs[query_param]
+            orm_filters[field_name] = self.kwargs[query_param]  # type: ignore[attr-defined]
         return queryset.filter(**orm_filters)
 
-    def initialize_request(self, request, *args, **kwargs):
+    def initialize_request(self, request: HttpRequest, *args: Any, **kwargs: Any) -> Request:
         """
         Adds the parent params from URL inside the children data available
         """
-        request = super().initialize_request(request, *args, **kwargs)
-        
+        drf_request: Request = super().initialize_request(request, *args, **kwargs)  # type: ignore[misc]
+
         if getattr(self, 'swagger_fake_view', False):
-            return request
+            return drf_request
 
         for url_kwarg, fk_filter in self._get_parent_lookup_kwargs().items():
             # fk_filter is alike 'grandparent__parent__pk'
             parent_arg = fk_filter.partition('__')[0]
-            for querydict in [request.data, request.query_params]:
+            for querydict in [drf_request.data, drf_request.query_params]:
                 with _force_mutable(querydict):
                     querydict[parent_arg] = kwargs[url_kwarg]
-        return request
+        return drf_request
```

### Comparing `drf-nested-routers-0.93.5/setup.py` & `drf-nested-routers-0.94.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import re
 import os
 import sys
 from setuptools import setup
 
 
 name = 'drf-nested-routers'
@@ -55,16 +54,16 @@
 if sys.argv[-1] == 'publish':
     if os.system("pip freeze | grep wheel"):
         print("wheel not installed.\nUse `pip install wheel`.\nPress <Enter> to continue or <Ctrl+C> to abort.")
         input()
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     print("You probably want to also tag the version now:")
-    print("  git tag -a v{0} -m 'version {0}'".format(version))
-    print("  git push origin v{0}".format(version))
+    print(f"  git tag -a v{version} -m 'version {version}'")
+    print(f"  git push origin v{version}")
     sys.exit()
 
 
 setup(
     name=name,
     version=version,
     url=url,
```

