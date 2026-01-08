FROM python:3.12

WORKDIR /app

COPY . .

RUN pip install uv

RUN uv sync

EXPOSE 8000

CMD ["uv", "run", "fastapi", "dev", "main.py", "--host", "0.0.0.0"]
