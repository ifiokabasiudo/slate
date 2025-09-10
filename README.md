# Slate CMS  

A lightweight, customizable **Content Management System** built with **Next.js, Supabase, and Docker**, designed to give non-technical users control over their websites. With **authentication, media management, and real-time content updates**, Slate CMS makes it simple for admins to manage content while keeping the app scalable and secure.  

---

## ✨ Features
- 🔐 **Authentication & Authorization**  
  - Admin login powered by Supabase Auth (JWT-based).  
  - Row Level Security (RLS) and custom policies for secure data access.  

- 📝 **Content Management**  
  - Admins can edit **text, images, and videos** on the site in real-time.  
  - Media stored securely in Supabase buckets.  

- 🎥 **Video Upload & Compression**  
  - Large video files are automatically compressed with **FFmpeg** while maintaining quality.  
  - Efficient storage & streaming for end users.  

- ⚡ **CI/CD Pipeline**  
  - Automated deployments using **GitHub Actions**.  
  - Build & push Docker images to **DockerHub**.  
  - Deploy backend services to **AWS EC2** with best practices.  

- 🌐 **DevOps & Infrastructure**  
  - Reverse proxy with **Nginx**.  
  - Azure OIDC integration with GitHub org for secure provider setup.  

---

## 🧠 Project Motivation
This project started while building a client website. Instead of a static site, I wanted to create a **scalable system** that gave the client full control over their content. The goal was to:  
- Learn how to integrate **Supabase buckets & RLS policies** for media and content storage.  
- Explore **video compression pipelines** with FFmpeg.  
- Gain real-world experience in **DevOps, CI/CD pipelines, and cloud deployments**.  

---

## 🏗️ How It Was Built
- **Frontend**: Next.js + Tailwind CSS for a responsive, dynamic admin dashboard.  
- **Backend**: Node.js + FFmpeg service for video compression.  
- **Database & Auth**: Supabase with RLS for granular security.  
- **CI/CD**: GitHub Actions for test → build → push → deploy automation.  
- **Cloud Deployment**:  
  - **AWS EC2** running Amazon Linux 2023.  
  - **Docker** for containerization.  
  - **Azure OIDC** for secure identity provider setup.  

---

## 📚 What I Learned
- How to design a **CMS architecture** with real-time content editing.  
- Handling **large media files** efficiently with FFmpeg & Supabase.  
- Setting up **secure RLS policies** and JWT-based auth.  
- Automating deployment pipelines with **GitHub Actions + Docker + AWS**.  
- Managing cloud infrastructure with **Nginx + OIDC** integrations.  

---

## 🛠️ Tech Stack
- **Frontend**: Next.js, Tailwind CSS  
- **Backend**: Node.js, FFmpeg  
- **Database & Auth**: Supabase (RLS + Buckets + JWT)  
- **DevOps**: GitHub Actions, Docker, DockerHub  
- **Cloud Hosting**: AWS EC2 (Amazon Linux 2023), Azure OIDC  
- **Web Server**: Nginx

---

## ⚡ Getting Started (Local Development)

```bash
# Clone the repository
git clone https://github.com/thesimpleprogramme/slate-cms.git
cd slate-cms

# Install dependencies
npm install

# Set up environment variables for Supabase and backend services
cp .env.example .env.local

# Run the app
npm run dev
