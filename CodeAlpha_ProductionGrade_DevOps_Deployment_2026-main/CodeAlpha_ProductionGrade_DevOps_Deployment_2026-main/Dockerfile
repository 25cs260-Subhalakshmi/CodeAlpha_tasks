FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html

HEALTHCHECK --interval=30s --timeout=5s CMD wget --spider -q http://localhost || exit 1

EXPOSE 80