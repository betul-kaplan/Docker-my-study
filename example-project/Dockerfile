FROM nginx:latest
LABEL maintainer="Betul Kaplan"
ENV USER="Betul"
ARG RENK
RUN apt-get update && apt-get install -y curl htop wget
WORKDIR /gecici
ADD https://wordpress.org/latest.tar.gz .
WORKDIR /usr/share/nginx/html 
COPY html/${RENK} .
CMD ["./script.sh"]
