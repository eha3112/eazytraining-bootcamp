FROM python:3.6-alpine
LABEL maintainer="El Hacene" 
WORKDIR /opt
COPY requirements.txt /opt/
RUN pip install --no-cache-dir -r requirements.txt
COPY app.py /opt/
COPY templates /opt/templates/
COPY static /opt/static/

ENV ODOO_URL="https://www.odoo.com"
ENV PGADMIN_URL="https://www.pgadmin.org"
EXPOSE 8080
ENTRYPOINT ["python"]
CMD ["app.py"]
