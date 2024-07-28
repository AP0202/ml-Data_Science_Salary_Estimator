docker build -t data-science-salary-prediction-service:v1 .

docker run -it --rm -p 9696:9696  data-science-salary-prediction-service:v1

Open another command prompt and paste this url curl -X GET http://127.0.0.1:9696/predict