FROM node:23-alpine
LABEL author="Ronald Bulbow" \
      creation_date="Dec/07/2024" \
      description="Web application developed node"

WORKDIR /home/node/app

COPY app /home/node/app

RUN <<EOF
mkdir -p /home/node/app/node_modules
chown -R node:node /home/node/app
npm install
EOF

USER node

EXPOSE 8080

CMD ["node","app.js"]


