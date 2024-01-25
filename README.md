
<style>
    ol {
    width: min(60rem, 90%);
    margin-inline: auto;

    display: flex;
    flex-wrap: wrap;
    gap: 2rem;

    list-style: none;
    counter-reset: cardnr;
    justify-content: center;
}

li {
    --frontColor: white;
    --width: 10em;
    --inlineP: 0.5rem;
    --borderR: 4rem;

    counter-increment: cardnr;
    width: calc(var(--width) - var(--inlineP) * 2);
    display: grid;
    grid-template:
        "icon" var(--borderR) "title"
        "descr" 1fr;
    margin-inline: var(--inlineP);
    margin-bottom: calc(var(--borderR));
    position: relative;
}

li .title,
li .descr {
    background: var(--frontColor);
    padding-inline: 1rem;
    padding-bottom: 1rem;
}

li .title {
    color: var(--accent-color);
    text-align: center;
    padding-bottom: 0.5rem;
}

li .title,
li .descr {
    filter: drop-shadow(0.125rem 0.125rem 0.075rem rgba(0, 0, 0, 0.25));
}

li .title {
    grid-area: title;
    font-size: 1.1rem;
    font-weight: bold;
}

li .descr {
    grid-area: descr;
    font-size: 0.85rem;
    text-align: center;
    color: black;
}

li .descr::before {
    content: "";
    width: var(--arrowW);
    height: var(--arrowH);
    position: absolute;
    right: 1.5rem;
    top: 100%;
    background: inherit;
    clip-path: polygon(0 0, 100% 0, 50% 100%);
}

li::after {
    content: counter(cardnr, decimal-leading-zero);
    position: absolute;
    z-index: -1;

    left: calc(var(--inlineP) * -1);
    right: calc(var(--inlineP) * -1);
    top: var(--borderR);
    bottom: calc(var(--borderR) * -1);

    display: flex;
    align-items: flex-end;
    background: var(--accent-color);
    background-image: linear-gradient(160deg,
            rgba(255, 255, 255, 0.25),
            transparent 25% 75%,
            rgba(0, 0, 0, 0.25));

    --pad: 1rem;
    padding: var(--pad);
    font-size: calc(var(--borderR) - var(--pad) * 2);
    color: white;
}

li::before {
    content: "";
    position: absolute;
    height: var(--borderR);
    top: calc(100% + var(--borderR) - 2px);
    left: calc(var(--inlineP) * -1);
    right: calc(var(--inlineP) * -1);
    border-radius: 0 var(--borderR) 0 0;

    background-image: linear-gradient(var(--accent-color), transparent 60%);
    opacity: 0.5;
    filter: blur(2px);
}
</style>

# FULL STACK DEVELOPER
<a href="https://www.jjcp.space" target="_blank">
    <picture>
        <!-- AVIF format for modern browsers that support it -->
        <source srcset="assets/logo.avif" type="image/avif">
        <!-- WebP format for modern browsers -->
        <source srcset="assets/logo.webp" type="image/webp">
        <!-- JPEG format for older browsers -->
        <img src="assets/logo.png" alt="jjcp.space">
    </picture>
</a>

# Hi, I'm Javier! 👋

I am Javier Cornejo, a fullstack developer who brings innovation and efficiency to the heart of projects. I've learned about Software Development and best practices through courses in my university and I've worked in various projects that allowed me to improve my skills with practice.

## 🛠 Expertise

<ol>
    <li style="--accent-color:#354c7c">
        <div class="title">BACKEND</div>
        <div class="descr">Most experiencie in backend</div>
    </li>
    <li style="--accent-color:#505a74">
        <div class="title">FRONTEND</div>
        <div class="descr">Freelance and first jobs as frontend</div>
    </li>
    <li style="--accent-color:#b0b8ce">
        <div class="title">DEVOPS</div>
        <div class="descr">Experience using AWS cloud</div>
    </li>
    <li style="--accent-color:#BDBEBE">
        <div class="title">SECURITY</div>
        <div class="descr">TDD, OWASP, LINUX</div>
    </li>
</ol>

## ⚡️ Skills

**Code:**  Javascript, Typescript, Java, Python, Golang, CSS, SASS, HTML, GraphQL, gRPC, Json.

**Stack:** NodeJS, ReactJS, Express, Angular, NestJS, NextJS, Django, LernaJS, Figma, Spring, Nginx, Docker.

**Repository:** Git, GitLab, GitHub, Jira, AzureDevOps.

**DB:** Mongo, PostgreSQL, redis, DocumentDB.

**Cloud:** AWS (ECR,ECS,Lambda, SQS, SNS, Step Function...) certified, Digital Ocean, Firebase.

**Concepts:** Scrum, Microservices, Design Patterns, Monorepo.

## 🔗 How to reach me

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://www.jjcp.space)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/javier-jail-cornejo)
[![portfolio](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/shionAoi)
[![twitter](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:javier.jail.cornejo@gmail.com)