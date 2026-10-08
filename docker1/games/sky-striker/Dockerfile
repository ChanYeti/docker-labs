# Build path : /root/games/sky-striker
# Build      : docker build -t chanyeti/game-skystriker:1.0 .
FROM nginx:alpine
LABEL org.opencontainers.image.title="Sky Striker" \
      org.opencontainers.image.description="HTML5 vertical scrolling shooter game served by nginx" \
      build.path="/root/games/sky-striker"
WORKDIR /usr/share/nginx/html
RUN rm -rf ./*
COPY index.html .
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
