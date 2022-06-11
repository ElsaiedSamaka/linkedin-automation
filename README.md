# Linkedin EasyApply Bot
Automate the application process on LinkedIn(Easy Apply)
 

The run the bot install requirements
```bash
pip install -r requirements.txt
```

Enter your username, password, and search settings into the `config.yaml` file

```yaml
username: # Insert your username here
password: # Insert your password here

positions:
- # positions you want to search for
- # Another position you want to search for
- # A third position you want to search for

locations:
- # Location you want to search for
- # A second location you want to search in 

uploads:
 Resume: # PATH TO Resume 
 Cover Letter: # PATH TO cover letter
 Photo: # PATH TO photo
# Note file_key:file_paths contained inside the uploads section should be writted without a dash ('-') 

output_filename:
- # PATH TO OUTPUT FILE (default output.csv)

33blacklist:
- # Company names you want to ignore
```


### Uploads

There is no limit to the number of files you can list in the uploads section. 
The program takes the titles from the input boxes and tries to match them with 
list in the config file.

## Execute

You can execute the bot by running the following in your terminal

## Notes

The bot will run by default for 10 hours and will sleep to make sure everything loads, have also  added random to make us look human.

on your root folder create output.csv file to avoid errors

```
## Notes
python3 easyapplybot.py
python easyapplybot.py

```

```
