<div align="center">
  
# 🕷️ Crawl4AI - Web Crawler & Scraper

### *Intelligent Web Crawling with AI-Powered Features*

[![Docker Pulls](https://img.shields.io/docker/pulls/unclecode/crawl4ai)](https://hub.docker.com/r/unclecode/crawl4ai)
[![GitHub Stars](https://img.shields.io/github/stars/unclecode/crawl4ai)](https://github.com/unclecode/crawl4ai)
[![License](https://img.shields.io/github/license/unclecode/crawl4ai)](https://github.com/unclecode/crawl4ai)

</div>

---

## 📋 Table of Contents
- [🚀 Quick Start with Docker](#-quick-start-with-docker)
- [🛠️ Method 1: Build from Source](#️-method-1-build-from-source)
- [🐳 Method 2: Pull from Docker Hub](#-method-2-pull-from-docker-hub)
- [🎯 Access Dashboard](#-access-dashboard)
- [📊 Features](#-features)

---

## 🚀 Quick Start with Docker

Choose your preferred method to run Crawl4AI:

| Method | Description | Best For |
|--------|-------------|----------|
| **Build from Source** | Clone repo & build locally | Development & customization |
| **Pull from Docker Hub** | Use pre-built image | Quick setup & production |

---
# 🐳 Method 1: Pull from Docker Hub

### Step 1: Pull the Official Image
Pull latest Crawl4AI image from Docker Hub
```
docker pull unclecode/crawl4ai:latest
```
### Step 2: Run the Container
Run the pre-built image
```
docker run -d \
  -p 11235:11235 \
  --name crawl4ai \
  --shm-size=1g \
  unclecode/crawl4ai:latest
```
## 🌐 Access Dashboard
Once the container is running, access the Crawl4AI web dashboard:
```
 http://localhost:11235/dashboard
```


# 🛠️ Method 2: Build from Source

### Step 1: Clone Repository

```
# Clone the Crawl4AI repository
git clone https://github.com/unclecode/crawl4ai.git

# Navigate to project directory
cd crawl4ai
```
### Step 2: Build Docker Image
```
# Build image for your current architecture
docker buildx build -t crawl4ai-local:latest --load .
```
### Step 3: Run the Container
```
# Run the container with optimized settings
docker run -d \
  -p 11235:11235 \
  --name crawl4ai-local \
  --shm-size=1g \
  crawl4ai-local:latest
```
## Step 3: Quick Commands Reference
```
# Stop the container
docker stop crawl4ai

# Start the container
docker start crawl4ai

# Remove the container
docker rm crawl4ai

# View real-time logs
docker logs -f crawl4ai
```

## Dashboard Features:
✅ Interactive web crawling interface

✅ Real-time scraping preview

✅ Configuration management

✅ Results visualization

✅ API testing playground

## 📊 Features
Feature	Description
🤖 AI-Powered	Intelligent content extraction
🔄 Dynamic Content	Handles JavaScript-rendered pages
📱 Responsive	Mobile-friendly dashboard
🚀 High Performance	Optimized with shared memory
🔒 Production Ready	Dockerized for easy deployment
