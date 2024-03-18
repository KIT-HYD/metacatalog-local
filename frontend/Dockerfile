FROM ghcr.io/hydrocode-de/metacatalog-ingest

# Fix the polars issue:
# the local machine is too old and the CPU is not supported
# thus we use polars-lts-cpu instead of polars
RUN pip uninstall polars
RUN pip install polars-lts-cpu

CMD ["python", "server.py"]
