FROM python:3.10
WORKDIR /code
ADD requirements.txt /code/
RUN pip install -r requirements.txt
# RUN⇒イメージのカスタマイズ
# requirements.txtに記述してあるものをまとめてpip
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
# python magage.py runserver 0.0.0.0:8000
# 上記コマンドを最初に一回実行する状態