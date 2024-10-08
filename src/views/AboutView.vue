<template>
  <div class="about">
    <div class="content">
      <div class="image-section">
        <img src="@/assets/myProfileImage.jpeg" alt="About Me Image" />
      </div>
      <div class="text-section">
        <h1>ABOUT ME</h1>
        <h3>Full Stack Developer</h3>
        <p>
          With a strong foundation in both frontend and backend development, I
          bring expertise in technologies like PHP, Python, C#, and database
          management. I specialize in developing APIs, real-time dashboards, and
          system integrations, continuously improving my skill set to deliver
          cutting-edge solutions. My approach combines technical precision with
          a deep understanding of user needs, ensuring that each project is both
          functional and impactful.
        </p>
        <div class="social-media">
          <a
            id="instagram-link"
            href="https://www.instagram.com/"
            target="_blank"
            rel="noopener noreferrer"
          >
            <i class="fab fa-instagram"></i>
          </a>
          <a
            id="linkedin-link"
            href="https://www.linkedin.com/in/felipegreghi/"
            target="_blank"
            rel="noopener noreferrer"
          >
            <i class="fab fa-linkedin"></i>
          </a>
          <a
            id="github-link"
            href="https://github.com/FelipeGreghi"
            target="_blank"
            rel="noopener noreferrer"
          >
            <i class="fab fa-github"></i>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutMe',
}
</script>

<style scoped>
@keyframes slideInRight {
  from {
    transform: translateX(100%);
    opacity: 0;
  }
  to {
    transform: translateX(0);
    opacity: 1;
  }
}
.about {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 10%;
}

.content {
  display: flex;
  border-radius: 8px;
}

.image-section img {
  max-width: 250px;
  max-height: 500px;
  border-top-left-radius: 8px;
  border-bottom-left-radius: 8px;
}

.text-section {
  flex: 2;
  padding: 2rem;
  animation: slideInRight 1.2s ease-in-out;
}

.text-section h1 {
  font-size: 2.75rem;
  font-weight: bold;
}

.text-section h3 {
  color: #46babe;
}

.text-section p {
  margin-top: 1rem;
  line-height: 1.6;
  font-size: 16px;
}

.social-media {
  display: flex;
  gap: 1rem;
}

.social-media a {
  color: inherit;
  text-decoration: none;
  font-size: 1.5rem;
}

#linkedin-link:hover {
  color: #0077b5; /* Cor de hover para LinkedIn */
}

#instagram-link:hover {
  color: #e1306c; /* Cor de hover para Instagram */
}

#github-link:hover {
  color: #ad3f11; /* Cor de hover para GitHub */
}

@media (max-width: 768px) {
  .content {
    flex-direction: column;
    align-items: center;
  }

  .image-section img {
    margin-top: 1rem;
    max-height: 350px;
    max-width: 175px;
    border-radius: 8px 8px 0 0;
  }

  .text-section {
    padding: 1rem;
  }

  .text-section h1 {
    font-size: 2rem;
  }

  .text-section p {
    font-size: 14px;
  }

  .social-media {
    justify-content: center;
  }
}

@media (max-width: 480px) {
  .image-section img {
    max-width: 80%;
  }

  .text-section h1 {
    font-size: 1.5rem;
  }

  .text-section p {
    font-size: 12px;
  }

  .social-media a {
    font-size: 1.5rem;
  }
}
</style>
