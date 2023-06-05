ARG VERSION=latest

# Fetching version dynamically by using arg instruction at the build time 
FROM ubuntu:$VERSION

LABEL EMAIL="kumar5483reddy@gmail.com" 

# Declaring arg and env 
ARG VERSION
ENV NAME APP_NAME
ENV PASSWORD APP_PASSWORD

WORKDIR /kumar

COPY . /kumar
ADD https://dlcdn.apache.org/maven/maven-3/3.8.6/source/apache-maven-3.8.6-src.tar.gz .
ADD apache-maven-3.8.6-src.tar.gz .

RUN echo $VERSION > image_version

# CMD ["echo", "Hello PAPA"]
# CMD ["echo", "Hello MAMA"]
# CMD ["echo", "Hello Boy"]

# ENTRYPOINT ["echo", "Hello World"]
# ENTRYPOINT ["sleep", "2"]

# When we use both at run time cmd as input to write and overwrite
CMD ["echo", "World"]
ENTRYPOINT ["echo", "Hello"]

EXPOSE 80