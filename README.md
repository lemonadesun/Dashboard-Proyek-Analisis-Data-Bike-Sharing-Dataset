# Dashboard-Proyek-Analisis-Data-Bike-Sharing-Dataset

# Setup environment
!pip install -q streamlit

!npm install localtunnel

# Run streamlit app
import urllib
print("Password/Enpoint IP for localtunnel is:",urllib.request.urlopen('https://ipv4.icanhazip.com').read().decode('utf8').strip("\n"))

!streamlit run /content/bike.py &>/content/logs.txt &

!npx localtunnel --port 8501
