# Using Python to Interact with the Operating System

Certificate of the course that is offered at Coursera and Google.

![Using Python to Interact with the Operating System](https://user-images.githubusercontent.com/41291493/109020226-2127ec00-76fd-11eb-8e43-e318af40d9f3.png)

## Learning Objectives
* Managing Files with Python
* Regular Expressions
* Advanced Regular Expressions
* Managing Data and Processes
* Bash Scripting

### Note

```
# Regex tool website
https://regex101.com/

re.sub(r"\b(\d{3})-(\d{3})-(\d{4})\b",r"+1-(\1) \2-\3",record)

pattern = "\w+[aeiouAEIOU]\w*[aeiouAEIOU]\w*[aeiouAEIOU]\w+"
result = re.findall(pattern, text)

result = re.sub('#+','//',line_of_code)

result = re.sub(r"\b(\d{3})-(\d{3})-(\d{4})\b",r"(\1) \2-\3",phone)

def check_web_address(text):
  pattern = r"\w\.com$|\.org|\.US"
  result = re.search(pattern, text)
  return result != None

def check_time(text):
  pattern = "(1[012]|[1-9]):"+ "[0-5][0-9](\\s)"+ "?(?i)(am|pm)";
  result = re.search(pattern, text)
  return result != None
  
def contains_acronym(text):
  pattern = r" [(I-M)]" 
  result = re.search(pattern, text)
  return result != None
```

## Credit

* [Certification-Link](https://www.coursera.org/account/accomplishments/verify/EZZYZ8GDRHHV)
