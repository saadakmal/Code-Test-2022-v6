# Code-Test-2022-v6
Code Test 2022 v6


Good Points:
-neat controller code, all business logic code is in repository.
-relations are used
-OOP concepts are used => inheritance, access modifiers, function overriding



Bad Points:
-Request validations weren't used
-Helper's directory was in wrong hierarchy
-Job Model was repeatedly called in Repository
-env() shouldn't be called directly in user editable code, 
    config() method should be used so that we can get only accessible params from .env
-This shouldn't be in .env file env('CUSTOMER_ROLE_ID'), instead use roles table from database
-Eager loading isn't utilized.
-many of the base methods of repository aren't used, it seems developer didn't kew they existed.
-coding styles -> camelCase and snake case both are used.

