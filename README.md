# mle-template-case-sprint2

Имя бакета: `s3-student-mle-20251120-23dfed9b96`

Проект в котором рассмотрены различные методы, улучшающие базовую модель предсказания цен на недвижимость. Проведен EDA анализ данных, выявляющий скрытые зависимости между признаками. Проведен Feature Engineering с помощью инструментов featuretools и AutoFeat с последующим отбором признаков методом Sequential Feature Selection. После работы с признаками подобраны гиперпараметры модели с помощью решетчатого поиска GridSearch и байесовского подхода в Optuna. Этапы совершенствования модели и ее версии зарегистрированы в MLflow Registry


Для начала работы с репозиторием необходимо настроить окружение:
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Пример файла окружения:
```
DB_DESTINATION_HOST=your_db_destination_host
DB_DESTINATION_PORT=your_db_destination_port
DB_DESTINATION_NAME=your_db_destination_name
DB_DESTINATION_USER=your_db_destination_user
DB_DESTINATION_PASSWORD=your_db_destination_password

S3_BUCKET_NAME=your_s3_bucket_name
AWS_ACCESS_KEY_ID=your_aws_access_key_id
AWS_SECRET_ACCESS_KEY=your_aws_secret_access_key
MLFLOW_S3_ENDPOINT_URL=your_mlflow_s3_endpoint_url

EXPERIMENT_NAME=your_experiment_name
```