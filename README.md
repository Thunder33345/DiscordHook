# DiscordHook
PHP Discord WebHook Library
Simple, All Cointained in One file!

Example:

To send a massage...
```php
DiscordHook::send(new Massage(new User("WEBHOOK URL", "USERNAME", "AVARAR_URL"), "MSG"));
```

Need to upload a file or embed(s)? DiscordHook Support that too!

Upload a File...
```php
DiscordHook::send(new Massage(new User("WEBHOOK URL", "USERNAME", "AVARAR_URL"), "MSG",new Upload("PATH TO FILE","FILE NAME")));
```

Send With Embed(s)...
```php
print_r(DiscordHook::send(new Massage(new User("WEBHOOK URL", "USERNAME", "AVARAR_URL"), "MSG",new Embed("TITLE","DESCRIPTION","URL","COLOUR(int)")))); //single embed
print_r(DiscordHook::send(new Massage(new User("WEBHOOK URL", "USERNAME", "AVARAR_URL"), "MSG",[new Embed("TITLE","DESCRIPTION","URL","COLOUR(int)"),new Embed("TITLE2","DESCRIPTION","URL","COLOUR(int)")]))); //multiple embeds
```
