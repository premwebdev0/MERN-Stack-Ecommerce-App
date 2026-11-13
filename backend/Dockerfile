FROM node:18-alpine
WORKDIR /app/backend
ENV NODE_ENV=production
COPY backend/package.json backend/package-lock.json ./
RUN npm ci --omit=dev || npm install --omit=dev
COPY backend/ ./
CMD ["node", "index.js"]
