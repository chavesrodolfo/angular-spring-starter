FROM nginx:1.13.3-alpine

## Copy our default nginx config
COPY nginx/default.conf /etc/nginx/conf.d/

## Remove default nginx website
RUN rm -rf /usr/share/nginx/html/*

## Copy dist content
COPY dist /usr/share/nginx/html

CMD ["nginx", "-g", "daemon off;"]