# Internationalization(i18n)
For intenational users, you have to use i18n variables for internationalization when you put text.

Required text is following languages.
- English
- Japanese

## Where to put messages
Administration console
- English: <service-admin>/src/main/resources/i18n/messages.properties
- Japanese: <service-admin>/src/main/resources/i18n/messages_ja.properties

For service api, i18 is not needed.

## Naming Convention
- variable name : [name for feature].[title for text]
- separating words : CamelCase

example: ```authentication.notFound = 'User with email not found'```

## Reference
Internationalization (i18n) with Spring
https://g00glen00b.be/spring-internationalization-i18n/
