FROM kittygram_final_frontend as build


FROM nginx:1.22.1
COPY nginx.conf /etc/nginx/templates/default.conf.template
COPY --from=build /app/build /static
EXPOSE 9000