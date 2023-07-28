**Steps of Connection :**

1) First open OpenAI platform using following link :
https://auth0.openai.com/u/login/identifier?state=hKFo2SBfeXJhT1lvOWlBUEhsZzliLVVmekVVbnlHOW5JaUU5b6Fur3VuaXZlcnNhbC1sb2dpbqN0aWTZIDA1RlZqT2xJcnFzQjFWV2lOVzBQdWNSX1hQOUN6Tk45o2NpZNkgRFJpdnNubTJNdTQyVDNLT3BxZHR3QjNOWXZpSFl6d0Q
2) Then sign in into OpenAI platform
3) After signing in you will able to see OpenAI Interface. In OpenAI Interface click on “Create new secret key”.
4) Then name the secret key and you will see your key.
5) After getting key first copy it and save it in file with any variable with any
name with extension .toml. TOML is a file format for configuration files. It
is intended to be easy to read and write due to obvious semantics which
aim to be "minimal", and is designed to map unambiguously to a dictionary.
Secrets.toml file :
api_secret = “your_key”
6) Put that file in C Disk in streamlit library :
C:\Users\Deepak\.streamlit\secrets.toml
7) Then write your python code, import essential libraries and paste your key in :
openai.api_key = st.secrets["api_secret"]
8) Then write your logic in code.
9) Run your file using cmd : streamlit run chatbot.py
10) Make sure that you are connected with internet.
