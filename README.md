# Sakthi Vignesh S – Portfolio Website

This project is a modern, responsive portfolio website built with HTML and CSS, designed with a yellow/white card-based theme. The site showcases my profile, projects, skills, certifications, and contact information.

## Dockerized Deployment

To make deployment easy and scalable, I created a `Dockerfile` that packages the static site (HTML, CSS, and image assets) into a Docker image using Nginx as the web server.

### Steps Followed

1. **Created the Portfolio Website**
   - Designed and implemented `index.html` and `style.css` for a visually appealing, card-based layout.
   - Added a profile image (`sakthi.jpg`).

2. **Dockerized the Site**
   - Wrote a `Dockerfile` to serve the static files using Nginx.
   - Built the Docker image locally.

3. **Pushed to Docker Hub**
   - Tagged and pushed the image to my Docker Hub repository: [`sakthi1607/sakthi-img:v1`](https://hub.docker.com/r/sakthi1607/sakthi-img)

4. **Deployed on Google Cloud Run**
   - Pulled the Docker image from Docker Hub in Google Cloud Run.
   - Configured Cloud Run for automatic deployment and scaling.



## How to Deploy

1. **Clone this repository**
2. **Build the Docker image:**
   ```powershell
   docker build -t sakthi1607/sakthi-img:v1 .
   ```
3. **Push to Docker Hub:**
   ```powershell
   docker push sakthi1607/sakthi-img:v1
   ```
4. **Deploy on Google Cloud Run:**
   - Create a new service in Cloud Run.
   - Use the image `sakthi1607/sakthi-img:v1`.
   - Set the container port to `80`.
   - Deploy and access your portfolio at the generated URL.

---

**Author:** Sakthi Vignesh S
