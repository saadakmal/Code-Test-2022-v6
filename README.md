# Code-Test-2022-v6

<h3>Good Points:</h3>
- Neat controller code, all business logic code is in repository.
- Relations are used.
- OOP concepts are used => inheritance, access modifiers, function overriding

<h3>Bad Points:</h3>
- Request validations weren't used.
- Helper's directory was in wrong hierarchy.
- Job Model was repeatedly called in Repository.
- env() shouldn't be called directly in user editable code, config() method should be used so that we can get only accessible params from .env.
- This shouldn't be in .env file env('CUSTOMER_ROLE_ID'), instead use roles table from database.
- Eager loading isn't utilized.
- Many of the base methods of repository aren't used, it seems developer didn't kew they existed.
- Coding styles -> camelCase and snake case both are used.
- Method return types missing where method is defined.
- Many of the functions comments were missing, they could be added to describe what it does to it easier for new devs.
- Select clause not used or rarely used.


<h3 style="color: green">How I would've done it:</h3>
- Use getter/setter methods
- Use Select clause where I know what data needs to be retrieved from database
- Add function's return type and enforce it.
- Write comments to describe method.
- Add comments at the top of file to utilize PHPStorm's auto discover features.
- For Example:
* @method string getService()
* @method string setService(string $service)
* @method array setEmailAddresses(array $email_addresses)
* @method string setSubject(string $setSubject)
* @method void setViewFileAndData(string $view, array $data)


