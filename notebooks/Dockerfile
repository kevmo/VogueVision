# Use an official Python base image
FROM python:3.11

# Set the working directory
WORKDIR /usr/src/app

# Copy the Pipfile and Pipfile.lock
COPY Pipfile Pipfile.lock ./

# Install pipenv and dependencies
RUN pip install pipenv && pipenv install --deploy --ignore-pipfile

# Copy the notebook files
COPY . .

# Expose the port Jupyter will run on
EXPOSE 8888

# Start Jupyter Notebook
CMD ["pipenv", "run", "jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
