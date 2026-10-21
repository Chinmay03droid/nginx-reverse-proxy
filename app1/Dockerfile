FROM python:3.13-slim
WORKDIR /app
RUN useradd --create-home appuser

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY --chown=appuser:appuser . .
USER appuser
EXPOSE 5001
CMD ["python", "app.py"]
