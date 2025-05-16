<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio - RAMIANDRISOA FANAMBINANA ADRIANO | Génie Électrique</title>
  <meta name="description" content="Portfolio professionnel de RAMIANDRISOA FANAMBINANA ADRIANO, étudiant en génie électrique réalisateur audio-visio et graphiste spécialisé en électronique et programmation">
  <meta name="keywords" content="portfolio, génie électrique, électronique, programmation,realisateur, Madagascar, développeur, ingénieur">
  <meta name="author" content="RAMIANDRISOA FANAMBINANA ADRIANO">
  <link rel="canonical" href="https://www.portfolio-ramsadry/informaticien.com"/>
  
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link href="https://fonts.googleapis.com/css2?family=Alex+Brush&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Person",
    "name": "RAMIANDRISOA FANAMBINANA ADRIANO",
    "alternateName": "ramsadry",
    "jobTitle": "Étudiant en génie Électronique des signaux et systèmes",
    "url": "https://www.ramsadry.com",
    "sameAs": [
      "https://app.netlify.com/teams/ramsadry-adriano/builds"
      "https://www.linkedin.com/in/ramsadry",
      "https://github.com/ramsadry/projets-publics",
      "https://www.facebook.com/ramsadry"
    ],
    "address": {
      "@type": "Tsiadana 026 A bis",
      "addressLocality": "Antananarivo",
      "addressCountry": "Madagascar"
    }
  }
  </script>

  <style>
    :root {
      --primary-color: #2c5364;
      --secondary-color: #203a43;
      --accent-color: #FFD700;
      --dark-color: #0f2027;
      --light-color: #f8f8f8;
      --text-color: #333;
      --error-color: #e74c3c;
      --logo-icon-size: 24px; /* Taille de l'icône du logo */
    }
    
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    
    body {
      font-family: 'Poppins', sans-serif;
      background-color: #f4f4f4;
      color: var(--text-color);
      line-height: 1.6;
      scroll-behavior: smooth;
    }

    /* Contenu principal */
    .portfolio-content {
      display: none; /* Modifié par JS pour être visible */
    }
    
    .portfolio-content.visible {
      display: block;
    }
    
    /* Header */
    .hero {
      background: linear-gradient(135deg, var(--dark-color), var(--secondary-color), var(--primary-color));
      color: white;
      padding: 120px 20px 50px;
      text-align: center;
      position: relative;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      clip-path: polygon(0 0, 100% 0, 100% 90%, 0 100%);
      margin-bottom: 30px;
    }
    
    @media (min-width: 768px) {
      .hero {
        perspective: 1px;
        transform-style: preserve-3d;
        overflow-x: hidden;
        overflow-y: auto;
      }
    }
    
    .hero::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: url('background-pattern.png') center/cover;
      opacity: 0.1;
      z-index: -1;
      transform: translateZ(-1px) scale(1.2);
    }
    
    .profile-pic {
      width: 160px;
      height: 160px;
      border-radius: 50%;
      border: 5px solid white;
      object-fit: cover;
      margin: 0 auto 20px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.3);
      transition: transform 0.4s ease, box-shadow 0.4s ease;
      animation: float 6s ease-in-out infinite;
    }
    
    @keyframes float {
      0% { transform: translateY(0px) rotate(0deg); }
      50% { transform: translateY(-20px) rotate(5deg); }
      100% { transform: translateY(0px) rotate(0deg); }
    }
    
    .profile-pic:hover {
      transform: scale(1.08) rotate(5deg);
      box-shadow: 0 8px 20px rgba(0,0,0,0.4);
    }
    
    .hero h1 {
      font-size: 2.8em;
      margin-bottom: 10px;
      font-weight: 700;
      letter-spacing: 1px;
      background: linear-gradient(90deg, #fff, var(--accent-color), #fff);
      background-size: 200% auto;
      color: #000;
      background-clip: text;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: shine 3s linear infinite;
    }
    
    @keyframes shine {
      to {
        background-position: 200% center;
      }
    }
    
    .hero h4 {
      font-family: 'Alex Brush', cursive;
      font-size: 2em;
      margin-bottom: 10px;
      color: #f8f8f8;
    }
    
    .hero p {
      font-style: italic;
      font-size: 1.1em;
      color: var(--accent-color);
      margin-bottom: 0;
    }
    
    .title-banner {
      background-color: var(--primary-color);
      color: white;
      padding: 15px;
      text-align: center;
      font-weight: 600;
      font-size: 1.2em;
      letter-spacing: 1px;
      margin: 20px 0 30px;
      border-radius: 5px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    }
    
    /* Barre de recherche */
    .search-container {
      display: flex;
      justify-content: center;
      padding: 20px;
      background-color: var(--light-color);
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      position: sticky;
      top: 0;
      z-index: 100;
    }
    
    .search-bar {
      display: flex;
      width: 100%;
      max-width: 600px;
    }
    
    .search-bar input {
      flex: 1;
      padding: 12px 20px;
      border: 2px solid #ddd;
      border-radius: 30px 0 0 30px;
      font-size: 16px;
      outline: none;
      transition: all 0.3s;
    }
    
    .search-bar input:focus {
      border-color: var(--primary-color);
      box-shadow: 0 0 8px rgba(44, 83, 100, 0.3);
    }
    
    .search-bar button {
      padding: 12px 25px;
      background: linear-gradient(to right, var(--secondary-color), var(--primary-color));
      color: white;
      border: none;
      border-radius: 0 30px 30px 0;
      cursor: pointer;
      font-size: 16px;
      transition: all 0.3s;
    }
    
    .search-bar button:hover {
      background: linear-gradient(to right, #1a2f38, #244556);
    }

    .nav-logo-icon, .section-logo-icon {
        width: var(--logo-icon-size);
        height: var(--logo-icon-size);
        margin-right: 8px;
        vertical-align: middle;
    }
    
    /* Navigation */
    nav {
      background-color: var(--dark-color);
      position: sticky;
      top: 80px; /* Ajusté si la barre de recherche a une hauteur fixe */
      z-index: 99;
      box-shadow: 0 2px 15px rgba(0,0,0,0.2);
    }
    
    nav ul {
      list-style: none;
      padding: 0;
      margin: 0;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    
    nav ul li {
      margin: 0;
    }
    
    nav ul li a {
      color: white;
      text-decoration: none;
      padding: 18px 25px;
      display: inline-flex; /* Pour aligner l'icône et le texte */
      align-items: center; /* Pour aligner l'icône et le texte */
      font-weight: 500;
      letter-spacing: 0.5px;
      transition: all 0.3s;
      position: relative;
    }
    
    nav ul li a:hover {
      background-color: var(--primary-color);
    }
    
    nav ul li a::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 50%;
      width: 0;
      height: 3px;
      background: var(--accent-color);
      transition: all 0.3s;
    }
    
    nav ul li a:hover::after {
      width: 70%;
      left: 15%;
    }
    
    .back-to-top {
      position: fixed;
      bottom: 30px;
      right: 30px;
      background: var(--primary-color);
      color: white;
      width: 50px;
      height: 50px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 20px;
      cursor: pointer;
      box-shadow: 0 3px 10px rgba(0,0,0,0.3);
      opacity: 0;
      visibility: hidden;
      transition: all 0.3s;
      z-index: 100;
    }
    
    .back-to-top.active {
      opacity: 1;
      visibility: visible;
    }
    
    .back-to-top:hover {
      background: var(--secondary-color);
      transform: translateY(-3px);
    }
    
    /* Sections */
    section {
      padding: 60px 20px;
      max-width: 1100px;
      margin: 0 auto;
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.6s ease-out, transform 0.6s ease-out;
    }
    
    section.visible {
      opacity: 1;
      transform: translateY(0);
    }
    
    section h2 {
      text-align: center;
      font-size: 2.2em;
      margin-bottom: 40px;
      color: var(--primary-color);
      position: relative;
      display: flex; /* Pour aligner l'icône et le texte */
      align-items: center; /* Pour aligner l'icône et le texte */
      justify-content: center; /* Pour centrer le contenu */
    }
    
    section h2::after {
      content: '';
      display: block;
      width: 100px;
      height: 4px;
      background: var(--accent-color);
      margin: 15px auto 0; /* Ajusté */
      border-radius: 2px;
      position: absolute; /* Pour le positionner sous le texte */
      bottom: -20px; /* Ajusté */
      left: 50%;
      transform: translateX(-50%);
    }

    section h2 .section-logo-icon { /* Style pour l'icône dans le h2 */
        margin-right: 10px;
    }
    
    .section-content {
      background: white;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 3px 15px rgba(0,0,0,0.1);
    }

    .cv-link {
        display: block;
        margin-top: 20px;
        text-align: right;
        font-weight: bold;
    }
    .cv-link a {
        color: var(--primary-color);
        text-decoration: none;
        transition: color 0.3s;
    }
    .cv-link a:hover {
        color: var(--accent-color);
        text-decoration: underline;
    }
    
    /* À propos */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 30px;
    }
    
    .about-text {
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
    
    .about-text p {
      margin-bottom: 20px;
      line-height: 1.8;
    }
    
    .about-image {
      display: flex;
      align-items: center;
      justify-content: center;
    }
    
    .about-image img {
      max-width: 100%;
      border-radius: 8px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      transition: transform 0.3s;
    }
    
    .about-image img:hover {
      transform: scale(1.03);
    }
    
    /* Expérience */
    .timeline {
      position: relative;
      max-width: 800px;
      margin: 0 auto;
    }
    
    .timeline::before {
      content: '';
      position: absolute;
      top: 0;
      bottom: 0;
      left: 50%;
      width: 2px;
      background: var(--primary-color);
      transform: translateX(-50%);
    }
    
    .timeline-item {
      position: relative;
      margin-bottom: 40px;
    }
    
    .timeline-date {
      position: absolute;
      left: 50%;
      transform: translateX(-50%);
      background: var(--primary-color);
      color: white;
      padding: 5px 15px;
      border-radius: 20px;
      font-size: 0.9em;
      font-weight: 500;
      box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    }
    
    .timeline-content {
      width: calc(50% - 40px);
      padding: 20px;
      background: white;
      border-radius: 8px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    }
    
    .timeline-item:nth-child(odd) .timeline-content {
      margin-left: 0;
      margin-right: auto;
    }
    
    .timeline-item:nth-child(even) .timeline-content {
      margin-left: auto;
      margin-right: 0;
    }
    
    /* Formation */
    .education-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 30px;
    }
    
    .education-card {
      background: white;
      padding: 25px;
      border-radius: 8px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.1);
      transition: transform 0.3s, box-shadow 0.3s;
      position: relative;
      overflow: hidden;
    }
    
    .education-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 215, 0, 0.1), transparent);
      transition: 0.5s;
    }
    
    .education-card:hover::before {
      left: 100%;
    }
    
    .education-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    }
    
    .education-icon {
      width: 60px;
      height: 60px;
      background: var(--primary-color);
      color: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 24px;
      margin-bottom: 15px;
    }
    
    .education-card h3 {
      color: var(--primary-color);
      margin-bottom: 10px;
    }
    
    .education-card h4 {
      color: #666;
      font-weight: 500;
      margin-bottom: 10px;
      font-size: 1.1em;
    }
    
    /* Compétences */
    .skills-container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 20px;
    }
    
    .skill-card {
      background: white;
      padding: 25px;
      border-radius: 8px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.1);
      transition: transform 0.3s, box-shadow 0.3s;
      border-left: 4px solid var(--primary-color);
      position: relative;
      overflow: hidden;
    }
    
    .skill-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 215, 0, 0.1), transparent);
      transition: 0.5s;
    }
    
    .skill-card:hover::before {
      left: 100%;
    }
    
    .skill-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    }
    
    .skill-card h3 {
      color: var(--primary-color);
      margin-bottom: 15px;
      display: flex;
      align-items: center;
    }
    
    .skill-card h3 i {
      margin-right: 10px;
      color: var(--accent-color);
    }
    
    .skill-card ul {
      padding-left: 20px;
    }
    
    .skill-card ul li {
      margin-bottom: 8px;
    }
    
    /* Projets */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
      gap: 30px;
    }
    
    .project-card {
      background: white;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
      transition: transform 0.3s, box-shadow 0.3s;
      position: relative;
      /* overflow: hidden; /* Already present */
    }
    
    .project-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 215, 0, 0.1), transparent);
      transition: 0.5s;
    }
    
    .project-card:hover::before {
      left: 100%;
    }
    
    .project-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
    }
    
    .project-image {
      height: 200px;
      overflow: hidden;
      position: relative;
    }
    
    .project-image img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.5s;
    }
    
    .project-card:hover .project-image img {
      transform: scale(1.1);
    }
    
    .project-content {
      padding: 20px;
    }
    
    .project-content h3 {
      color: var(--primary-color);
      margin-bottom: 10px;
    }
    
    .project-content p {
      margin-bottom: 15px;
      color: #666;
    }
    
    .project-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 15px;
    }
    
    .project-tag {
      background: #f0f0f0;
      padding: 5px 10px;
      border-radius: 20px;
      font-size: 0.8em;
      color: #555;
    }
    
    .project-link {
      display: inline-block;
      padding: 8px 15px;
      background: var(--primary-color);
      color: white;
      text-decoration: none;
      border-radius: 4px;
      transition: background 0.3s;
    }
    
    .project-link:hover {
      background: var(--secondary-color);
    }
    
    /* Galerie */
    .gallery-container {
      position: relative;
      max-width: 1000px; /* Ajusté pour potentiellement plus d'images */
      margin: 0 auto;
    }
    
    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); /* Ajusté pour plus d'images */
      gap: 15px; /* Ajusté */
    }
    
    .gallery-item {
      position: relative;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 3px 10px rgba(0,0,0,0.2);
      cursor: pointer;
      transition: transform 0.3s;
      height: 180px; /* Hauteur fixe pour uniformité */
    }
    
    .gallery-item:hover {
      transform: scale(1.03);
    }
    
    .gallery-item img {
      width: 100%;
      height: 100%; /* Ajusté */
      object-fit: cover;
      display: block;
      transition: transform 0.5s;
    }
    
    .gallery-item:hover img {
      transform: scale(1.1);
    }
    
    .gallery-caption {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      background: rgba(0,0,0,0.7);
      color: white;
      padding: 10px;
      transform: translateY(100%);
      transition: transform 0.3s;
      font-size: 0.9em;
    }
    
    .gallery-item:hover .gallery-caption {
      transform: translateY(0);
    }
    
    /* Lightbox */
    .lightbox {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.9);
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 1000;
      opacity: 0;
      visibility: hidden;
      transition: all 0.3s;
    }
    
    .lightbox.active {
      opacity: 1;
      visibility: visible;
    }
    
    .lightbox-content {
      position: relative;
      max-width: 90%;
      max-height: 90%;
      display: flex; /* Pour centrer le média à l'intérieur */
      align-items: center;
      justify-content: center;
    }
    
    #lightboxMediaContainer {
        display: flex;
        align-items: center;
        justify-content: center;
        max-width: 100%;
        max-height: 100%;
    }

    #lightboxMediaContainer img, 
    #lightboxMediaContainer iframe {
      max-width: 100%; /* S'assure que l'image/vidéo ne dépasse pas le conteneur */
      max-height: 80vh; /* Limite la hauteur pour laisser de la place aux contrôles */
      border-radius: 8px;
      box-shadow: 0 5px 25px rgba(0,0,0,0.5);
      display: block; /* Pour s'assurer que les marges auto fonctionnent si besoin */
    }
     #lightboxMediaContainer iframe {
        width: 80vw; /* Largeur pour les vidéos */
        height: calc(80vw * 9 / 16); /* Maintien du ratio 16:9 */
        min-width: 300px; /* taille minimale pour petites videos */
        min-height: 168px;
    }

    @media (max-width: 768px) {
        #lightboxMediaContainer iframe {
            width: 90vw;
            height: calc(90vw * 9 / 16);
        }
    }
    
    .lightbox-close {
      position: absolute;
      top: -40px;  /* Ajusté pour être au-dessus du contenu agrandi */
      right: 0px; /* Ajusté pour être plus accessible */
      color: white;
      font-size: 30px;
      cursor: pointer;
      z-index: 1001; /* S'assurer qu'il est au-dessus du média */
    }
    
    .lightbox-nav {
      position: absolute;
      top: 50%;
      width: 100%;
      display: flex;
      justify-content: space-between;
      padding: 0 20px;
      transform: translateY(-50%);
      z-index: 1001; /* Au-dessus du média */
    }
    
    .lightbox-nav button {
      background: rgba(255,255,255,0.3);
      color: white;
      border: none;
      width: 50px;
      height: 50px;
      border-radius: 50%;
      font-size: 20px;
      cursor: pointer;
      transition: all 0.3s;
    }
    
    .lightbox-nav button:hover {
      background: rgba(255,255,255,0.5);
    }
    
    /* Contact */
    .contact-container {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 30px;
    }
    
    .contact-info {
      background: white;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 3px 15px rgba(0,0,0,0.1);
    }
    
    .contact-info h3 {
      color: var(--primary-color);
      margin-bottom: 20px;
      font-size: 1.5em;
    }
    
    .contact-details {
      margin-bottom: 30px;
    }
    
    .contact-item {
      display: flex;
      align-items: center;
      margin-bottom: 15px;
    }
    
    .contact-item i {
      width: 40px;
      height: 40px;
      background: var(--primary-color);
      color: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-right: 15px;
      font-size: 18px;
    }
    
    .social-links {
      display: flex;
      gap: 15px;
      margin-top: 20px;
    }
    
    .social-link {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 40px;
      height: 40px;
      background: var(--primary-color);
      color: white;
      border-radius: 50%;
      font-size: 18px;
      transition: all 0.3s;
      text-decoration: none;
    }
    
    .social-link:hover {
      background: var(--secondary-color);
      transform: translateY(-3px);
    }
    
    .contact-form {
      background: white;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 3px 15px rgba(0,0,0,0.1);
    }
    
    .form-group {
      margin-bottom: 20px;
    }
    
    .form-group label {
      display: block;
      margin-bottom: 8px;
      font-weight: 500;
      color: #555;
    }
    
    .form-group input,
    .form-group textarea {
      width: 100%;
      padding: 12px 15px;
      border: 2px solid #ddd;
      border-radius: 6px;
      font-size: 16px;
      transition: all 0.3s;
    }
    
    .form-group input:focus,
    .form-group textarea:focus {
      border-color: var(--primary-color);
      box-shadow: 0 0 8px rgba(44, 83, 100, 0.2);
      outline: none;
    }
    
    .form-group textarea {
      min-height: 150px;
      resize: vertical;
    }
    
    .submit-btn {
      padding: 12px 30px;
      background: linear-gradient(to right, var(--secondary-color), var(--primary-color));
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-size: 16px;
      font-weight: 500;
      transition: all 0.3s;
    }
    
    .submit-btn:hover {
      background: linear-gradient(to right, #1a2f38, #244556);
      transform: translateY(-2px);
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }
    
    /* Carte de contact */
    .contact-map {
      position: relative;
      height: 300px;
      margin-bottom: 30px;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }
    
    .contact-map iframe {
      width: 100%;
      height: 100%;
      border: none;
    }
    
    .map-overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(44, 83, 100, 0.7);
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-size: 1.2em;
      cursor: pointer;
      transition: all 0.3s;
    }
    
    .map-btn {
      position: absolute;
      bottom: 20px;
      right: 20px;
      padding: 10px 20px;
      background: var(--accent-color);
      color: var(--dark-color);
      border: none;
      border-radius: 30px;
      cursor: pointer;
      font-weight: 600;
      z-index: 10;
      box-shadow: 0 3px 10px rgba(0,0,0,0.2);
      transition: all 0.3s;
    }
    
    .map-btn:hover {
      transform: translateY(-3px);
      box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    }
    
    /* Options de liens */
    .link-options {
      background: white;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 3px 15px rgba(0,0,0,0.1);
      margin-bottom: 20px;
    }
    
    .link-options h3 {
      color: var(--primary-color);
      margin-bottom: 15px;
      font-size: 1.3em;
    }
    
    .link-selector {
      width: 100%;
      padding: 10px;
      border: 2px solid #ddd;
      border-radius: 6px;
      font-size: 16px;
      transition: all 0.3s;
    }
    
    .link-selector:focus {
      border-color: var(--primary-color);
      box-shadow: 0 0 8px rgba(44, 83, 100, 0.2);
    }
    
    /* Vidéo */
    .videos-grid-container { /* Nouveau conteneur pour la grille de vidéos */
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 20px;
        margin: 30px 0;
    }

    .video-container {
      position: relative;
      padding-bottom: 56.25%; /* 16:9 */
      height: 0;
      overflow: hidden;
      border-radius: 8px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      cursor: pointer; /* Ajouté pour indiquer la cliquabilité */
    }
    
    .video-container iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
      pointer-events: none; /* Pour que le clic passe au conteneur parent pour le lightbox */
    }
    
    /* Footer */
    footer {
      background: linear-gradient(135deg, var(--dark-color), var(--secondary-color));
      color: white;
      padding: 50px 20px 30px;
      margin-top: 60px;
      text-align: center;
      clip-path: polygon(0 10%, 100% 0, 100% 100%, 0 100%);
    }
    
    .footer-content {
      max-width: 1200px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
      text-align: left;
    }
    
    .footer-column h3 {
      font-size: 1.3em;
      margin-bottom: 20px;
      position: relative;
      display: inline-block;
    }
    
    .footer-column h3::after {
      content: '';
      position: absolute;
      bottom: -8px;
      left: 0;
      width: 50px;
      height: 3px;
      background: var(--accent-color);
    }
    
    .footer-column p {
      margin-bottom: 15px;
      opacity: 0.8;
    }
    
    .footer-links {
      list-style: none;
    }
    
    .footer-links li {
      margin-bottom: 10px;
    }
    
    .footer-links a {
      color: white;
      text-decoration: none;
      transition: all 0.3s;
      opacity: 0.8;
    }
    
    .footer-links a:hover {
      opacity: 1;
      padding-left: 5px;
      color: var(--accent-color);
    }
    
    .footer-social {
      display: flex;
      gap: 15px;
      margin-top: 20px;
    }
    
    .footer-bottom {
      margin-top: 40px;
      padding-top: 20px;
      border-top: 1px solid rgba(255,255,255,0.1);
    }
    
    /* Highlight de recherche */
    .highlight {
      background-color: var(--accent-color);
      color: var(--dark-color);
      padding: 0 3px;
      border-radius: 3px;
    }
    
    @keyframes highlightPulse {
      0% { transform: scale(1); box-shadow: none; }
      50% { transform: scale(1.02); box-shadow: 0 0 20px rgba(255, 215, 0, 0.3); }
      100% { transform: scale(1); box-shadow: none; }
    }
    
    /* Notifications */
    .notification {
      position: fixed;
      bottom: 20px;
      left: 50%;
      transform: translateX(-50%) translateY(100px);
      padding: 15px 25px;
      border-radius: 5px;
      color: white;
      display: flex;
      align-items: center;
      gap: 10px;
      z-index: 1000;
      opacity: 0;
      transition: all 0.3s ease;
    }
    
    .notification.show {
      transform: translateX(-50%) translateY(0);
      opacity: 1;
    }
    
    .notification.success {
      background: linear-gradient(135deg, #2ecc71, #27ae60);
      box-shadow: 0 3px 10px rgba(46, 204, 113, 0.3);
    }
    
    .notification.error {
      background: linear-gradient(135deg, #e74c3c, #c0392b);
      box-shadow: 0 3px 10px rgba(231, 76, 60, 0.3);
    }
    
    /* Sélecteur de thème */
    .theme-switcher {
      position: fixed;
      bottom: 30px;
      left: 30px;
      display: flex;
      gap: 10px;
      z-index: 100;
    }
    
    .theme-switcher button {
      padding: 8px 15px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      font-weight: 500;
      display: flex;
      align-items: center;
      gap: 8px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.2);
      transition: all 0.3s;
    }
    
    .theme-switcher button:hover {
      transform: translateY(-3px);
      box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    }
    
    /* Responsive */
    @media (max-width: 992px) {
      .about-grid,
      .contact-container {
        grid-template-columns: 1fr;
      }
      
      .about-image {
        order: -1;
      }
      
      .timeline::before {
        left: 30px;
      }
      
      .timeline-item {
        padding-left: 70px;
      }
      
      .timeline-date {
        left: 0;
        transform: none;
      }
      
      .timeline-content {
        width: 100%;
      }
      .videos-grid-container {
        grid-template-columns: 1fr; /* Une vidéo par ligne sur écrans moyens */
      }
    }
    
    @media (max-width: 768px) {
      .hero {
        padding: 100px 20px 40px;
        clip-path: polygon(0 0, 100% 0, 100% 95%, 0 100%);
      }
      
      .hero h1 {
        font-size: 2.2em;
      }
      
      nav ul li {
        width: 100%;
        text-align: center;
      }
      
      nav ul li a {
        padding: 15px;
        width: 100%;
        justify-content: center; /* Centrer icône et texte */
      }
      
      .projects-grid {
        grid-template-columns: 1fr;
      }
      
      .back-to-top {
        width: 40px;
        height: 40px;
        font-size: 16px;
        bottom: 20px;
        right: 20px;
      }
      
      .theme-switcher {
        bottom: 80px;
        flex-direction: column;
      }
      .gallery-grid {
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Plus petites images sur mobile */
      }
       section h2 {
        font-size: 1.8em; /* Taille de titre réduite pour mobile */
      }
      .nav-logo-icon, .section-logo-icon {
        var(--logo-icon-size): 20px; /* Icône plus petite sur mobile */
      }
    }
  </style>
</head>
<body>
  <div class="portfolio-content" id="portfolioContent"> <header class="hero">
      <img src="profil/profil.jpg" alt="Photo de profil de RAMIANDRISOA FANAMBINANA ADRIANO" loading="lazy" class="profile-pic">
      <h1>RAMIANDRISOA FANAMBINANA ADRIANO</h1>
      <h4>"Ramsadry"</h4>
      <p><em>Étudiant en génie électrique & passionné par la technologie</em></p>
      <p><em>GAMEUR ET GRAPHISTE</em></p>
    </header>

    <div class="title-banner">
      <p>CREATIF|EXPERT|PRATICANT</p> </div>
    
    <div class="search-container">
      <div class="search-bar">
        <input type="text" id="search-input" placeholder="Rechercher dans le portfolio...">
        <button id="search-btn"><i class="fas fa-search"></i></button> </div>
    </div>
    
    <nav>
      <ul>
        <li><a href="#about"><img src="logo-icon.png" alt="Logo" class="nav-logo-icon" onerror="this.style.display='none'"><i class="fas fa-user"></i> À propos</a></li>
        <li><a href="#experience"><img src="logo-icon.png" alt="Logo" class="nav-logo-icon" onerror="this.style.display='none'"><i class="fas fa-briefcase"></i> Expérience</a></li>
        <li><a href="#education"><img src="logo-icon.png" alt="Logo" class="nav-logo-icon" onerror="this.style.display='none'"><i class="fas fa-graduation-cap"></i> Formation</a></li>
        <li><a href="#skills"><img src="logo-icon.png" alt="Logo" class="nav-logo-icon" onerror="this.style.display='none'"><i class="fas fa-cogs"></i> Compétences</a></li>
        <li><a href="#projects"><img src="logo-icon.png" alt="Logo" class="nav-logo-icon" onerror="this.style.display='none'"><i class="fas fa-project-diagram"></i> Projets</a></li>
        <li><a href="#gallery"><img src="logo-icon.png" alt="Logo" class="nav-logo-icon" onerror="this.style.display='none'"><i class="fas fa-images"></i> Galerie</a></li>
        <li><a href="#video"><img src="logo-icon.png" alt="Logo" class="nav-logo-icon" onerror="this.style.display='none'"><i class="fas fa-video"></i> Vidéos</a></li>
        <li><a href="#contact"><img src="logo-icon.png" alt="Logo" class="nav-logo-icon" onerror="this.style.display='none'"><i class="fas fa-envelope"></i> Contact</a></li>
      </ul>
    </nav>

    <div class="theme-switcher">
      <button data-theme="light"><i class="fas fa-sun"></i> Clair</button>
      <button data-theme="dark"><i class="fas fa-moon"></i> Sombre</button>
      <button data-theme="blue"><i class="fas fa-water"></i> Bleu</button>
    </div>

    <div class="back-to-top" id="backToTop">
      <i class="fas fa-arrow-up"></i>
    </div>

    <section id="about">
      <h2><img src="logo-icon.png" alt="Icône" class="section-logo-icon" onerror="this.style.display='none'"><i class="fas fa-user"></i> À propos de moi</h2>
      <div class="section-content">
        <div class="about-grid">
          <div class="about-text">
            <p>Je m'appelle Adriano, étudiant passionné par l'électronique, la programmation et les systèmes embarqués. Mon parcours académique et mes projets personnels m'ont permis d'acquérir des compétences solides dans ces domaines.</p>
            <p>Curieux et autodidacte, j'aime relever de nouveaux défis techniques et développer des solutions innovantes. Mon objectif est de combiner mes connaissances en génie électrique avec mes compétences en développement pour créer des projets à la pointe de la technologie.</p>
            <p>En dehors de mes études, je me consacre à l'apprentissage continu, au partage de connaissances et au développement de projets personnels qui repoussent mes limites.</p>
             <p class="cv-link"><a href="circulum vitae.pdf" target="_blank">Acceder sur mon CV<i class="fas fa-external-link-alt"></i></a></p> </div>
          <div class="about-image">
            <img src="image/about-image.jpg" alt="Adriano au travail" loading="lazy">
          </div>
        </div>
      </div>
    </section>
    
    <section id="experience">
      <h2><img src="logo-icon.png" alt="Icône" class="section-logo-icon" onerror="this.style.display='none'"><i class="fas fa-briefcase"></i> Expérience Professionnelle</h2>
      <div class="section-content">
        <div class="timeline">
          <div class="timeline-item">
            <div class="timeline-date">2024 - Présent</div>
            <div class="timeline-content">
              <h3>Technicien en Électronique</h3>
              <h4>Entreprise Macro-farma, Antananarivo</h4>
              <ul>
                <li>Réparation et maintenance d'équipements électroniques</li>
                <li>Développement de solutions embarquées sur microcontrôleurs</li>
                <li>Assistance technique aux clients</li>
              </ul>
            </div>
          </div>
          <div class="timeline-item">
            <div class="timeline-date">2024 - 2025</div>
            <div class="timeline-content">
              <h3>Stagiaire en Génie Électrique</h3>
              <h4>Société ABC, Antananarivo</h4>
              <ul>
                <li>Participation à l'installation de systèmes électriques</li>
                <li>Tests et validation de circuits imprimés</li>
                <li>Documentation technique</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="education">
      <h2><img src="logo-icon.png" alt="Icône" class="section-logo-icon" onerror="this.style.display='none'"><i class="fas fa-graduation-cap"></i> Formation</h2>
      <div class="section-content">
        <div class="education-grid">
          <div class="education-card">
            <div class="education-icon">
              <i class="fas fa-university"></i>
            </div>
            <h3>Licence en Génie Électrique</h3>
            <h4>Université de Madagascar, 2023-2026</h4>
            <p>Spécialisation en systèmes embarqués et automatisme</p>
          </div>
          <div class="education-card">
            <div class="education-icon">
              <i class="fas fa-certificate"></i>
            </div>
            <h3>Certification en Développement Web</h3>
            <h4>Plateforme en ligne, 2023</h4>
            <p>HTML5, CSS3, JavaScript et frameworks modernes</p>
          </div>
        </div>
      </div>
    </section>

    <section id="skills">
      <h2><img src="logo-icon." alt="Icône" class="section-logo-icon" onerror="this.style.display='none'"><i class="fas fa-cogs"></i> Mes Compétences</h2>
      <div class="section-content">
        <div class="skills-container">
          <div class="skill-card">
            <h3><i class="fas fa-code"></i> Programmation</h3>
            <ul>
              <li>MATLAB (Simulink)</li>
              <li>Python (NumPy, Pandas)</li>
              <li>C/C++ (Arduino, STM32)</li>
              <li>JavaScript (Node.js)</li>
              <li>HTML5/CSS3</li>
            </ul>
          </div>
          <div class="skill-card">
            <h3><i class="fas fa-bolt"></i> Électronique</h3>
            <ul>
              <li>Conception de circuits</li>
              <li>Simulation SPICE</li>
              <li>Systèmes embarqués</li>
              <li>Microcontrôleurs</li>
              <li>Capteurs et actionneurs</li>
            </ul>
          </div>
          <div class="skill-card">
            <h3><i class="fas fa-tools"></i> Techniques</h3>
            <ul>
              <li>Installation électrique</li>
              <li>Réparation électronique</li>
              <li>Soudage CMS/THT</li>
              <li>Prototypage rapide</li>
              <li>Tests et dépannage</li>
            </ul>
          </div>
         <div class="skill-card">
            <h3><i class="fas fa-globe"></i>Réalisateur</h3>
            <ul>
              <li>maintenance de manipulation</li>
              <li>Travail d'équipe</li>
              <li>Résolution de problèmes</li>
              <li>Apprentissage d'instalation</li>
              <li>Montage audio-visio</li>
            </ul>
          </div>
          <div class="skill-card">
            <h3><i class="fas fa-globe"></i> Autres</h3>
            <ul>
              <li>Gestion de projet</li>
              <li>Travail d'équipe</li>
              <li>Résolution de problèmes</li>
              <li>Apprentissage continu</li>
              <li>Français, Anglais</li>
            </ul>
          </div>
        </div>
        <p class="cv-link"><a href="circulum vitae.pdf" target="_blank">Acceder sur mon CV <i class="fas fa-external-link-alt"></i></a></p> </div>
    </section>

    <section id="projects">
      <h2><img src="logo-icon.png" alt="Icône" class="section-logo-icon" onerror="this.style.display='none'"><i class="fas fa-project-diagram"></i> Mes Projets</h2>
      <div class="section-content">
        <div class="projects-grid">
          <div class="project-card">
            <div class="project-image">
              <img src="project/project1.jpg" alt="Simulation MATLAB" loading="lazy">
            </div>
            <div class="project-content">
              <h3>Simulation de circuits avec MATLAB</h3>
              <div class="project-tags">
                <span class="project-tag">MATLAB</span>
                <span class="project-tag">Simulink</span>
                <span class="project-tag">Électronique</span>
              </div>
              <p>Projet de simulation de filtres passe-bas en utilisant Simulink pour analyser les caractéristiques fréquentielles des circuits électroniques avec différentes configurations.</p>
              <a href="#" class="project-link">Voir plus</a>
            </div>
          </div>
          <div class="project-card">
            <div class="project-image">
              <img src="project/project2.png" alt="Site web personnel" loading="lazy">
            </div>
            <div class="project-content">
              <h3>Site web personnel</h3>
              <div class="project-tags">
                <span class="project-tag">HTML5</span>
                <span class="project-tag">CSS3</span>
                <span class="project-tag">JavaScript</span>
              </div>
              <p>Développement d'un portfolio responsive avec animations modernes pour présenter mes compétences et projets de manière professionnelle et interactive.</p>
              <a href="#" class="project-link">Voir plus</a>
            </div>
          </div>
          <div class="project-card">
            <div class="project-image">
              <img src="project/project3.jpg" alt="Installation électrique" loading="lazy">
            </div>
            <div class="project-content">
              <h3>Installation et réparation électrique</h3>
              <div class="project-tags">
                <span class="project-tag">Électricité</span>
                <span class="project-tag">Sécurité</span>
                <span class="project-tag">Dépannage</span>
              </div>
              <p>Installation complète de systèmes de caméras de surveillance et configuration de systèmes d'alarme, ainsi que déblocage et flashage d'appareils électroniques.</p>
              <a href="#" class="project-link">Voir plus</a>
            </div>
          </div>
        </div>
         <p class="cv-link"><a href="circulum vitae.pdf" target="_blank">Acceder sur mon CV <i class="fas fa-external-link-alt"></i></a></p> </div>
    </section>
    
    <section id="gallery">
      <h2><img src="logo-icon.png" alt="Icône" class="section-logo-icon" onerror="this.style.display='none'"><i class="fas fa-images"></i> Galerie Photo</h2>
      <div class="section-content">
        <div class="gallery-container">
          <div class="gallery-grid">
            <div class="gallery-item" data-media="photo1.jpg" data-media-type="image">
              <img src="image/photo1.jpg" alt="Projet électronique" loading="lazy">
              <div class="gallery-caption">Nouvelle photo1</div>
            </div>
            <div class="gallery-item" data-media="photo2.jpg" data-media-type="image">
              <img src="image/photo2.jpg" alt="Laboratoire" loading="lazy">
              <div class="gallery-caption">Nouvelle photo2</div>
            </div>
            <div class="gallery-item" data-media="photo3.jpg" data-media-type="image">
              <img src="image/photo3.jpg" alt="Installation électrique" loading="lazy">
              <div class="gallery-caption">Nouvelle photo3</div>
            </div>
            <div class="gallery-item" data-media="photo4.jpg" data-media-type="image">
              <img src="image/photo4.jpg" alt="Simulation" loading="lazy">
              <div class="gallery-caption">Nouvelle photo4</div>
            </div>
            <div class="gallery-item" data-media="photo5.jpg" data-media-type="image">
              <img src="image/photo5.jpg" alt="Projet Arduino" loading="lazy">
              <div class="gallery-caption">Nouvelle photo5</div>
            </div>
            <div class="gallery-item" data-media="photo6.jpg" data-media-type="image"> <img src="image/photo6.jpg" alt="Soudage" loading="lazy">
              <div class="gallery-caption">Nouvelle photo6</div>
            </div>
            <div class="gallery-item" data-media="photo7.jpg" data-media-type="image">
              <img src="image/photo7.jpg" alt="Placeholder Photo 7" loading="lazy">
              <div class="gallery-caption">Nouvelle Photo 7</div>
            </div>
            <div class="gallery-item" data-media="photo8.jpg" data-media-type="image">
              <img src="image/photo8.jpg" alt="Placeholder Photo 8" loading="lazy">
              <div class="gallery-caption">Nouvelle Photo 8</div>
            </div>
            <div class="gallery-item" data-media="photo9.jpg" data-media-type="image">
              <img src="image/photo9.jpg" alt="Placeholder Photo 9" loading="lazy">
              <div class="gallery-caption">Nouvelle Photo 9</div>
            </div>
            <div class="gallery-item" data-media="photo10.jpg" data-media-type="image">
              <img src="image/photo10.jpg" alt="Placeholder Photo 10" loading="lazy">
              <div class="gallery-caption">Nouvelle Photo 10</div>
            </div>
            <div class="gallery-item" data-media="photo11.jpg" data-media-type="image">
              <img src="image/photo11.jpg" alt="Placeholder Photo 11" loading="lazy">
              <div class="gallery-caption">Nouvelle Photo 11</div>
            </div>
            <div class="gallery-item" data-media="photo12.jpg" data-media-type="image">
              <img src="image/photo12.jpg" alt="Placeholder Photo 12" loading="lazy">
              <div class="gallery-caption">Nouvelle Photo 12</div>
            </div>
            <div class="gallery-item" data-media="photo13.jpg" data-media-type="image">
              <img src="image/photo13.jpg" alt="Placeholder Photo 13" loading="lazy">
              <div class="gallery-caption">Nouvelle Photo 13</div>
            </div>
            <div class="gallery-item" data-media="photo14.jpg" data-media-type="image">
              <img src="image/photo14.jpg" alt="Placeholder Photo 14" loading="lazy">
              <div class="gallery-caption">Nouvelle Photo 14</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <div class="lightbox" id="lightbox">
      <div class="lightbox-content">
        <span class="lightbox-close" id="lightboxClose">×</span>
        <div id="lightboxMediaContainer">
            </div>
        <div class="lightbox-nav">
          <button id="lightboxPrev"><i class="fas fa-chevron-left"></i></button>
          <button id="lightboxNext"><i class="fas fa-chevron-right"></i></button>
        </div>
      </div>
    </div>

    <section id="video">
      <h2><img src="logo-icon.png" alt="Icône" class="section-logo-icon" onerror="this.style.display='none'"><i class="fas fa-video"></i> Mes Vidéos</h2>
      <div class="section-content">
        <p style="text-align: center; margin-bottom: 30px;">Découvrez en vidéo mon parcours, mes compétences et quelques-uns de mes projets réalisés.</p>
        <div class="videos-grid-container">
            <div class="video-container" data-media-src="video1.mp4" data-media-type="video" title="Vidéo d'Aventure 1"> 
                <iframe src="video1.mp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen title="Vidéo d'Aventure 1"></iframe>
            </div>
            <div class="video-container" data-media-src="video2.mp4" data-media-type="video" title="Video d'Aventure 2">
              <iframe src="video2.mp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen title="Video d'Aventure 2"></iframe>
            </div>
            <div class="video-container" data-media-src="video3.mp4" data-media-type="video" title="Video d'Aventure 3">
              <iframe src="video3.mp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen title="Video d'Aventure 3"></iframe>
            </div>
            <div class="video-container" data-media-src="video4.mp4" data-media-type="video" title="Vidéo d'Aventure 4">
              <iframe src="video4.mp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen title="Vidéo d'Aventure 4"></iframe>
            </div>
            <div class="video-container" data-media-src="video5.mp4" data-media-type="video" title="Vidéo d'Aventure 5">
              <iframe src="video5.mp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen title="Vidéo d'Aventure 5"></iframe>
            </div>
        </div>
      </div>
    </section>

    <section id="contact">
      <h2><img src="logo-icon.png" alt="Icône" class="section-logo-icon" onerror="this.style.display='none'"><i class="fas fa-envelope"></i> Contactez-moi</h2>
      <div class="section-content">
        <div class="link-options">
          <h3>Options de liens</h3>
          <div class="form-group">
            <label for="linkedinOption">LinkedIn:</label>
            <select id="linkedinOption" class="link-selector">
              <option value="linkedin1">Profil personnel</option>
              <option value="linkedin2">Page professionnelle</option>
            </select>
          </div>
          <div class="form-group">
            <label for="githubOption">GitHub:</label>
            <select id="githubOption" class="link-selector">
              <option value="github1">Projets publics</option>
              <option value="github2">Projets académiques</option>
            </select>
          </div>
          <div class="form-group">
            <label for="youtubeOption">YouTube:</label>
            <select id="youtubeOption" class="link-selector">
              <option value="youtube1">Tutoriels</option>
              <option value="youtube2">Démonstrations</option>
            </select>
          </div>
        </div>

        <div class="contact-container">
          <div class="contact-info">
            <h3>Informations de contact</h3>
            <div class="contact-details">
              <div class="contact-item">
                <i class="fas fa-map-marker-alt"></i>
                <div>
                  <strong>Adresse</strong>
                  <p>Antananarivo 101 Tsiadana 026 A bis, Madagascar</p>
                </div>
              </div>
              <div class="contact-item">
                <i class="fas fa-envelope"></i>
                <div>
                  <strong>Email</strong>
                  <p>ramsadry3@gmail.com</p>
                </div>
              </div>
              <div class="contact-item">
                <i class="fas fa-phone"></i>
                <div>
                  <strong>Téléphone</strong>
                  <p>+261 38 54 962 35</p>
                </div>
              </div>
            </div>
            <h3>Réseaux sociaux</h3>
            <div class="social-links">
              <a href="https://www.facebook.com/ramsadry" class="social-link" target="_blank" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
              <a href="https://www.linkedin.com/in/profil-personnel" class="social-link" target="_blank" id="linkedinLink" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
              <a href="https://github.com/ramsadry/projets-publics" class="social-link" target="_blank" id="githubLink" aria-label="GitHub"><i class="fab fa-github"></i></a>
              <a href="https://youtube.com/ramsadry-tutoriels" class="social-link" target="_blank" id="youtubeLink" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
            </div>
          </div>
          <div class="contact-form">
            <form id="contactForm">
              <div class="form-group">
                <label for="name">Nom complet</label>
                <input type="text" id="name" required>
              </div>
              <div class="form-group">
                <label for="email">Adresse email</label>
                <input type="email" id="email" required>
              </div>
              <div class="form-group">
                <label for="subject">Sujet</label>
                <input type="text" id="subject" required>
              </div>
              <div class="form-group">
                <label for="message">Message</label>
                <textarea id="message" required></textarea>
              </div>
              <button type="submit" class="submit-btn"><i class="fas fa-paper-plane"></i> Envoyer</button>
            </form>
          </div>
        </div>
      </div>
    </section>

    <footer>
      <div class="footer-content">
        <div class="footer-column">
          <h3>À propos</h3>
          <p>Portfolio professionnel de RAMIANDRISOA FANAMBINANA ADRIANO, étudiant en génie électrique et passionné par la technologie.</p>
          <div class="footer-social">
            <a href="https://www.facebook.com/ramsadry" target="_blank" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
            <a href="https://www.linkedin.com/in/profil-personnel" target="_blank" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
            <a href="https://github.com/ramsadry/projets-publics" target="_blank" aria-label="GitHub"><i class="fab fa-github"></i></a>
            <a href="https://youtube.com/ramsadry-tutoriels" target="_blank" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
          </div>
        </div>
        <div class="footer-column">
          <h3>Liens rapides</h3>
          <ul class="footer-links">
            <li><a href="#about"><i class="fas fa-chevron-right"></i> À propos</a></li>
            <li><a href="#skills"><i class="fas fa-chevron-right"></i> Compétences</a></li>
            <li><a href="#projects"><i class="fas fa-chevron-right"></i> Projets</a></li>
            <li><a href="#gallery"><i class="fas fa-chevron-right"></i> Galerie</a></li>
            <li><a href="#contact"><i class="fas fa-chevron-right"></i> Contact</a></li>
          </ul>
        </div>
        <div class="footer-column">
          <h3>Contact</h3>
          <p><i class="fas fa-map-marker-alt"></i> Antananarivo, Madagascar</p>
          <p><i class="fas fa-envelope"></i> ramsadry3@gmail.com</p>
          <p><i class="fas fa-phone"></i> +261 38 54 962 35</p>
        </div>
      </div>
      <div class="footer-bottom">
        <p>© 2025 RAMIANDRISOA FANAMBINANA ADRIANO. Tous droits réservés.</p>
      </div>
    </footer>
  </div>

  <script>
    // Gestion de la connexion - SUPPRIMÉE

    // Options de liens
    const linkedinLinks = {
      'linkedin1': 'https://www.linkedin.com/in/profil-personnel',
      'linkedin2': 'https://www.linkedin.com/company/page-professionnelle' // Exemple
    };

    const githubLinks = {
      'github1': 'https://github.com/ramsadry/projets-publics',
      'github2': 'https://github.com/ramsadry/projets-academiques' // Exemple
    };

    const youtubeLinks = {
      'youtube1': 'https://youtube.com/ramsadry-tutoriels',
      'youtube2': 'https://youtube.com/ramsadry-demos'
    };

    document.querySelectorAll('.link-selector').forEach(select => {
      select.addEventListener('change', function() {
        const id = this.id;
        const value = this.value;
        
        if(id === 'linkedinOption') {
          document.getElementById('linkedinLink').href = linkedinLinks[value];
          document.querySelector('footer .footer-social a[aria-label="LinkedIn"]').href = linkedinLinks[value];
        } else if(id === 'githubOption') {
          document.getElementById('githubLink').href = githubLinks[value];
          document.querySelector('footer .footer-social a[aria-label="GitHub"]').href = githubLinks[value];
        } else if(id === 'youtubeOption') {
          document.getElementById('youtubeLink').href = youtubeLinks[value];
          document.querySelector('footer .footer-social a[aria-label="YouTube"]').href = youtubeLinks[value];
        }
      });
    });

    // Back to top button
    const backToTopBtn = document.getElementById('backToTop');
    
    window.addEventListener('scroll', () => {
      if (window.pageYOffset > 300) {
        backToTopBtn.classList.add('active');
      } else {
        backToTopBtn.classList.remove('active');
      }
    });
    
    backToTopBtn.addEventListener('click', () => {
      window.scrollTo({
        top: 0,
        behavior: 'smooth'
      });
    });
    
    // Lightbox functionality (Modifié pour images et vidéos)
    const lightbox = document.getElementById('lightbox');
    const lightboxMediaContainer = document.getElementById('lightboxMediaContainer'); // Modifié
    const lightboxClose = document.getElementById('lightboxClose');
    const lightboxPrev = document.getElementById('lightboxPrev');
    const lightboxNext = document.getElementById('lightboxNext');
    
    let currentMediaIndex = 0;
    let mediaElements = []; // Stocke les éléments (images et vidéos) pour la lightbox
    
    function updateGalleryAndVideoItems() {
        const imageGalleryItems = Array.from(document.querySelectorAll('.gallery-item[data-media-type="image"]'));
        const videoGalleryItems = Array.from(document.querySelectorAll('.video-container[data-media-type="video"]'));

        mediaElements = [
            ...imageGalleryItems.map(item => ({ 
                element: item, 
                type: 'image', 
                src: item.getAttribute('data-media'),
                title: item.querySelector('.gallery-caption') ? item.querySelector('.gallery-caption').textContent : ''
            })),
            ...videoGalleryItems.map(item => ({ 
                element: item, 
                type: 'video', 
                src: item.getAttribute('data-media-src'),
                title: item.getAttribute('title') || ''
            }))
        ];

        mediaElements.forEach((media, index) => {
            media.element.removeEventListener('click', openLightboxHandler); // Éviter les doubles écouteurs
            // Wrapper pour passer l'index correctement à l'handler
            const handler = (event) => {
                // Pour les conteneurs vidéo, s'assurer que le clic sur l'iframe ne déclenche pas une double action
                // ou n'empêche pas l'ouverture du lightbox. pointer-events: none sur l'iframe gère cela.
                openLightboxHandler(index);
            };
            media.element.addEventListener('click', handler);
        });
    }
    
    function openLightboxHandler(index) {
        currentMediaIndex = index;
        const media = mediaElements[currentMediaIndex];
        openLightbox(media.src, media.type, media.title);
    }

    function openLightbox(mediaSrc, mediaType = 'image', mediaTitle = '') {
      lightboxMediaContainer.innerHTML = ''; // Vider le contenu précédent
      
      if (mediaType === 'video') {
        const iframe = document.createElement('iframe');
        iframe.setAttribute('src', mediaSrc);
        iframe.setAttribute('frameborder', '0');
        iframe.setAttribute('allow', 'accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture');
        iframe.setAttribute('allowfullscreen', 'true');
        iframe.setAttribute('title', mediaTitle || 'Vidéo');
        // Les styles pour l'iframe sont dans le CSS #lightboxMediaContainer iframe
        lightboxMediaContainer.appendChild(iframe);
      } else { // image
        const img = document.createElement('img');
        img.src = mediaSrc;
        img.alt = mediaTitle || 'Image agrandie';
        // Les styles pour l'image sont dans le CSS #lightboxMediaContainer img
        lightboxMediaContainer.appendChild(img);
      }
      
      lightbox.classList.add('active');
      document.body.style.overflow = 'hidden'; // Empêcher le défilement de l'arrière-plan
    }
    
    function closeLightbox() {
      lightbox.classList.remove('active');
      document.body.style.overflow = 'auto'; // Rétablir le défilement
      lightboxMediaContainer.innerHTML = ""; // Vider la source pour arrêter les vidéos/gifs
    }
    
    function showPrevMedia() {
      currentMediaIndex = (currentMediaIndex - 1 + mediaElements.length) % mediaElements.length;
      const media = mediaElements[currentMediaIndex];
      openLightbox(media.src, media.type, media.title);
    }
    
    function showNextMedia() {
      currentMediaIndex = (currentMediaIndex + 1) % mediaElements.length;
      const media = mediaElements[currentMediaIndex];
      openLightbox(media.src, media.type, media.title);
    }
    
    lightboxClose.addEventListener('click', closeLightbox);
    lightboxPrev.addEventListener('click', showPrevMedia);
    lightboxNext.addEventListener('click', showNextMedia);
    
    lightbox.addEventListener('click', (e) => {
      // Fermer si on clique sur le fond noir (lightbox elle-même)
      if (e.target === lightbox) {
        closeLightbox();
      }
    });
    
    document.addEventListener('keydown', (e) => {
      if (lightbox.classList.contains('active')) {
        if (e.key === 'Escape') {
          closeLightbox();
        } else if (e.key === 'ArrowLeft') {
          showPrevMedia();
        } else if (e.key === 'ArrowRight') {
          showNextMedia();
        }
      }
    });
    
    // Search functionality
    const searchInput = document.getElementById('search-input');
    const searchBtn = document.getElementById('search-btn');
    
    function highlightText(element, text) {
      const walker = document.createTreeWalker(element, NodeFilter.SHOW_TEXT, null, false);
      let node;
      const regex = new RegExp(text, 'gi');
      const nodesToReplace = [];

      while (node = walker.nextNode()) {
          if (node.nodeValue.toLowerCase().includes(text.toLowerCase())) {
              nodesToReplace.push(node);
          }
      }

      nodesToReplace.forEach(textNode => {
          const parent = textNode.parentNode;
          if (parent.nodeName === 'SCRIPT' || parent.nodeName === 'STYLE') return; // Ne pas modifier script/style

          const fragment = document.createDocumentFragment();
          let lastIndex = 0;
          textNode.nodeValue.replace(regex, (match, offset) => {
              fragment.appendChild(document.createTextNode(textNode.nodeValue.substring(lastIndex, offset)));
              const span = document.createElement('span');
              span.className = 'highlight';
              span.textContent = match;
              fragment.appendChild(span);
              lastIndex = offset + match.length;
          });
          fragment.appendChild(document.createTextNode(textNode.nodeValue.substring(lastIndex)));
          parent.replaceChild(fragment, textNode);
      });
    }
    
    function removeHighlights() {
      document.querySelectorAll('span.highlight').forEach(highlight => {
        const parent = highlight.parentNode;
        parent.replaceChild(document.createTextNode(highlight.textContent), highlight);
        parent.normalize(); // Fusionner les nœuds texte adjacents
      });
    }
    
    function searchContent() {
      const searchTerm = searchInput.value.trim(); 
      
      removeHighlights(); // Toujours retirer les highlights précédents

      if (searchTerm === '') {
        // showNotification('Veuillez entrer un terme de recherche', false); // Optionnel: notifier si vide
        return;
      }
      
      const elementsToSearch = document.querySelectorAll('section .section-content, .project-card .project-content, .skill-card, .timeline-item .timeline-content, .education-card, .hero');
      let found = false;
      let firstMatch = null;
      
      elementsToSearch.forEach(element => {
        const text = element.textContent; 
        if (text.toLowerCase().includes(searchTerm.toLowerCase())) {
          found = true;
          highlightText(element, searchTerm); 
          
          element.style.animation = 'highlightPulse 1.5s ease-out';
          setTimeout(() => {
            element.style.animation = '';
          }, 1500);
          
          if (!firstMatch) {
            firstMatch = element;
          }
        }
      });
      
      if (found && firstMatch) {
        const rect = firstMatch.getBoundingClientRect();
        const isVisible = (
            rect.top >= 0 &&
            rect.left >= 0 &&
            rect.bottom <= (window.innerHeight || document.documentElement.clientHeight) &&
            rect.right <= (window.innerWidth || document.documentElement.clientWidth)
        );

        if (!isVisible) {
            firstMatch.scrollIntoView({
              behavior: 'smooth',
              block: 'center' 
            });
        }
        showNotification(`Des résultats ont été trouvés pour "${searchTerm}"`);
      } else if (searchTerm !== '') { // Ne pas notifier si la recherche était vide initialement
        showNotification(`Aucun résultat trouvé pour "${searchTerm}"`, false);
      }
    }
    
    searchBtn.addEventListener('click', searchContent);
    searchInput.addEventListener('keypress', (e) => {
      if (e.key === 'Enter') {
        searchContent();
      }
    });
    
    // Form submission
    const contactForm = document.getElementById('contactForm');
    
    contactForm.addEventListener('submit', (e) => {
      e.preventDefault();
      
      const name = document.getElementById('name').value;
      const email = document.getElementById('email').value;
      const subject = document.getElementById('subject').value;
      const message = document.getElementById('message').value;
      
      console.log('Formulaire soumis:', { name, email, subject, message });
      showNotification(`Merci ${name}, votre message a été envoyé avec succès !`);
      contactForm.reset();
    });
    
    // Smooth scrolling for navigation links
    document.querySelectorAll('nav a').forEach(anchor => {
      anchor.addEventListener('click', function(e) {
        e.preventDefault();
        
        const targetId = this.getAttribute('href');
        const targetElement = document.querySelector(targetId);
        
        if (targetElement) {
          const navHeight = document.querySelector('nav').offsetHeight;
          const searchBarHeight = document.querySelector('.search-container') ? document.querySelector('.search-container').offsetHeight : 0;
          const offset = navHeight + searchBarHeight + 20; 

          window.scrollTo({
            top: targetElement.offsetTop - offset,
            behavior: 'smooth'
          });
        }
      });
    });

    // Notification system
    function showNotification(message, isSuccess = true) {
      const notification = document.createElement('div');
      notification.className = `notification ${isSuccess ? 'success' : 'error'}`;
      notification.innerHTML = `
        <i class="fas fa-${isSuccess ? 'check-circle' : 'exclamation-circle'}"></i>
        <span>${message}</span>
      `;
      document.body.appendChild(notification);
      
      setTimeout(() => {
        notification.classList.add('show');
      }, 10);
      
      setTimeout(() => {
        notification.classList.remove('show');
        setTimeout(() => {
          notification.remove();
        }, 500);
      }, 3000);
    }

    // Theme switcher
    document.querySelectorAll('.theme-switcher button').forEach(btn => {
      btn.addEventListener('click', function() {
        const selectedTheme = this.dataset.theme;
        document.body.className = selectedTheme + '-theme'; 
        localStorage.setItem('portfolio-theme', selectedTheme);
      });
    });

    // Apply saved theme on load
    const savedTheme = localStorage.getItem('portfolio-theme') || 'light';
    document.body.className = savedTheme + '-theme'; 

    // Observer pour animer les sections au scroll
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
          observer.unobserve(entry.target); 
        }
      });
    }, {threshold: 0.1});

    document.querySelectorAll('section').forEach(section => {
      observer.observe(section);
    });

    // Initialiser après le chargement du DOM
    document.addEventListener('DOMContentLoaded', () => {
        document.getElementById('portfolioContent').classList.add('visible'); // Rendre le contenu visible
        if(document.getElementById('loginContainer')) { // Au cas où il n'a pas été supprimé du HTML pour une raison
            document.getElementById('loginContainer').style.display = 'none';
        }
        
        updateGalleryAndVideoItems(); // Initialiser la galerie et les vidéos pour la lightbox
        
        // Appliquer le thème sauvegardé
        const currentTheme = localStorage.getItem('portfolio-theme') || 'light';
        document.body.className = currentTheme + '-theme';
    });

  </script>
</body>
</html>
