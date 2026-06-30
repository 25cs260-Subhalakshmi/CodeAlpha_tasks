FROM nginx:alpine

LABEL maintainer="Subhalakshmi Bagavathiraj"
LABEL project="Azure DevOps CI/CD Pipeline"
LABEL description="Cloud-native containerized web application deployment"

COPY app/index.html /usr/share/nginx/html/index.html

EXPOSE 80

HEALTHCHECK --interval=30s --timeout=5s --start-period=10s --retries=3 \
CMD wget --quiet --tries=1 --spider http://localhost || exit 1