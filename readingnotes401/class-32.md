# Permissions in Django

Permissions are checked at the very beginning before code is ran. The purpose: to make sure the person accessing is properly vetted and allowed to access the content and resources. Combined with throttling and authentication, the API will be able to determine if content should be sent or if an error should be thrown.

## Steps to Access

Permission checks are typically initiated with request.user and request.auth properties to see if requests can come through. The requests will approve or deny the user access to all or parts of the classes in an API.

## Permission Levels

User level permissions use the IsAuthenticated class as the simplest way to determine user eligibility. The IsAuthenticatedOrReadOnly class will give full access to those authenticated and read only access to those unauthenticated.

Tests for exceptions.PermissionDenied and exceptions.NotAuthenticated need to pass prior to the body of the code being ran. Return if not authenticated will be a 403 Forbidden or a 401 Unauthorized error majority of time.

Object level permissions check user access to object level. Typically the model instance using .get_object(). If you are creating your own views, you will need to specifically call .check_object_permissions(request, obj) method on the view at the point of which you’re retrieving the object permissions. As with user level, an error will be thrown if unauthorized.

Except for DjangoObjectPermissions, the built in permissions from rest_framework.permissions don’t necessarily check the object permissions. To use the rest_framework object permissions you will need to subclass them and use has_object_permission(). The check for permissions will need to be in your serializer or override perform _create() method in viewpoint set.

## Things I want to know more about

### Resources

[DRF](https://www.django-rest-framework.org/api-guide/permissions/#django-rest-framework-api-key)

### Links

- >[Advanced Software Development](README.md)
