# CI/CD Node.js App with Docker

This is a simple Node.js application set up with Docker and GitHub Actions for Continuous Integration and Deployment.

## Project Structure
- `backend/`: Node.js application and Dockerfile
- `.github/workflows/ci.yml`: GitHub Actions CI/CD pipeline
- `docker-compose.yml`: Local development setup (optional)

## Directory Structure
ci-cd-node-app/
├── backend/                  # <- Backend app folder
│   ├── Dockerfile            # <- Dockerfile for backend app
│   ├── server.js             # <- Main server code (Node.js)
│   └── package.json          # <- Node.js dependencies
├── docker-compose.yml        # <- Optional for local development
├── .github/                  # <- GitHub Actions folder
│   └── workflows/            # <- GitHub Actions workflows
│       └── ci.yml            # <- CI/CD pipeline file
├── README.md                 # <- Project readme file


## Getting Started

### Prerequisites
- Docker
- DockerHub Account
- GitHub Account

### Running Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/ci-cd-node-app.git

2. Build and run the Docker Container:
   docker-compose up --build

3. Access the app at http://localhost:3000

4. Deployment
   This app is automatically deployed to DockerHub whenever you push to the main branch on GitHub.

5. License: MIT License.   

---

### 8️⃣ **Final Check**:

1. **Backend Code**:
   - `Dockerfile` & `server.js` ko backend folder mein rakha.
   - `package.json` mein dependencies define ki.
  
1. **Backend Code:**
   - Placed Dockerfile and server.js inside the backend directory.
   - Defined dependencies in package.json.

2. **GitHub Actions CI/CD Pipeline:**
   - Configured .github/workflows/ci.yml to build the Docker Image and push it to Docker Hub.

3. **Docker Setup:**
   - Ensured the Dockerfile is located inside the backend directory.

4. **Secrets:**
   - Added DOCKER_USERNAME and DOCKER_PASSWORD to GitHub Secrets.

---

### 🏁 **Push & Test**

1. **Push the code to GitHub**:
   ```bash
   git add .
   git commit -m "Initial setup of CI/CD pipeline"
   git push origin main

