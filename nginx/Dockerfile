FROM nginx:stable-alpine

RUN rm /etc/nginx/conf.d/default.conf

COPY nginx.conf /etc/nginx/nginx.conf
COPY proxy.conf /etc/nginx/conf.d/default.conf
COPY proxy_params /etc/nginx/proxy_params

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

