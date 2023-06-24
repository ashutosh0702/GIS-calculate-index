# Base image
FROM public.ecr.aws/lambda/python:3.9


# Copy the source code and requirements file
COPY src/lambda_function.py ${LAMBDA_TASK_ROOT}
COPY src/requirements.txt ${LAMBDA_TASK_ROOT}


# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Set the entry point
CMD ["lambda_function.lambda_handler"]

