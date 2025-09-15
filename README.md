<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>ΔCosmofaee // Accueil</title>
    <link rel="stylesheet" href="https://dl.dropbox.com/scl/fi/mi7w0owzv7xpyd9xnygi1/stylesheetp.css?rlkey=nwa4g3bfz2ad53qzlbda359nw">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Michroma&family=Tektur:wght@400..900&display=swap" rel="stylesheet">
    <!-- INSTALLATION DE FONT ICON -->
    <link href="https://code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css" rel="stylesheet"/>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.4.0/font/bootstrap-icons.css">
	<link rel="stylesheet" href="https://code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css">
</head>
<body>
    <div class="fond">
        <div class="titre_accueil"><a href="index.html">Archive_ΔCosmofaee</a></div>

        <div class="hautbas">
            <span><a href="#top">↑</a></span>
            <span><a href="#bottom">↓</a></span>
        </div>

        <!-- Lightbox -->
        <div id="lightbox" class="lightbox">
            <span class="close"></span>
            <img class="lightbox-content" id="lightbox-img">
        </div>

        <div class="conteneur">
            <div class="carte_identite">
                <span class="ci_texte">Adrien Feraud</span>
                <span class="ci_img"><img src="https://i59.servimg.com/u/f59/19/69/15/66/moi10.jpg" alt="Photo d'Adrien Feraud"></span>
                <span class="ci_texte">Portfolio</span>
            </div>

            <div class="ci_presentation">
                Passionné par les jeux vidéo, je m’intéresse à l’ensemble des secteurs du domaine, de la conception à la production. Bénéficiaire de la RQTH. Je suis reconnu pour mon sérieux, mon implication et ma créativité. Curieux et motivé, je cherche à mettre mes compétences au service de projets stimulants.
            </div>

            <div class="menu">
                <span><a href="conceptart.html">Concept Art</a></span>
                <span><a href="ecriture.html">Écriture</a></span>
                <span><a href="jeux.html">Jeux</a></span>
                <span><a href="code.html">Code</a></span>
            </div>

            <div class="second_conteneur">
                <div class="titre">Mes dernières créations</div>
                <div class="der_crea">
                    <div class="der_article"><span><img src="https://i72.servimg.com/u/f72/20/55/53/24/qherth10.jpg" class="zoomable"></span><span>Particulièrement inspiré pour ce monstre, j'ai voulu pour mon forum une créature plus puissante que toutes celles qui existent, une bête dont les joueurs pourront avoir réellement peur et douter de pouvoir l'abattre.</span></div>
                    <div class="der_article"><span><img src="https://i72.servimg.com/u/f72/20/55/53/24/captur13.png" class="zoomable"></span><span>J'ai récemment codé pour mon forum RPG un répertoire qui réunit toutes les créations inventées par les joueurs. Il contient des armes et des objets avec des fonctionalités différentes, qui se lient même ensemble pour certains. Chaque petite carte comporte toutes les informations concernant l'objet.</span></div>
                    <div class="der_article"><span><img src="https://i72.servimg.com/u/f72/20/55/53/24/adrien10.jpg" class="zoomable"></span><span>Sur un instagram, j'ai vu passer un post montrant l'affiche de <u>Perfect Blue</u> et proposant aux artistes de se faire dessus avec leur persona. J'ai profité alors de cette occasion pour tenter un nouveau style.</span></div>
                </div>
            </div>

            <div class="titre">Mes inspirations</div>
            <div class="inspi">
                Je puise mon inspiration de beaucoup d'auteurs et d'oeuvres différents, ceux qui m'ont donné la passion du jeu vidéo, de l'écriture et de l'horreur.<br>
                Je pense d'abord à <u>Odysseas Theodoratos</u>, avec son webcomic <u>Tomahawk Angel</u> pour ses concepts de monstres originaux et terrifiants.<br>
                La franchise <u>Monster Hunter</u> a aussi été une grande source d'inspiration pour ses créatures riches en détails.<br>
                <u>Junji Ito</u> est le magaka que j'admire le plus, que ce soit pour son style ou sa créativité dans ses écrits.<br>
                Le jeu <u>Stray</u> pour ses décors et son atmosphère de solitude et pourtant colorés à certains endroits.<br>
                Puis la série de livres <u>La Guerre des Clans</u> par <u>Erin Hunter</u> qui est celle qui m'a transmise la passion pour l'écriture.<br>
                Et bien entendu, <u>League Of Legends</u>, dont les cinématiques et l'univers sont particulièrement riches et qui a été le premier à me donner cet envie de travailler dans le milieu du jeu vidéo.
            </div>
        </div>
    </div>

    <script>
        //POUR LE ZOOM SUR LES IMAGES
        const lightbox = document.getElementById("lightbox");
        const lightboxImg = document.getElementById("lightbox-img");
        const closeBtn = document.querySelector(".lightbox .close");

        document.querySelectorAll(".zoomable").forEach(img => {
        img.addEventListener("click", () => {
            lightbox.style.display = "flex";
            lightboxImg.src = img.src;
        });
        });

        // fermer avec la croix
        closeBtn.addEventListener("click", () => {
        lightbox.style.display = "none";
        });

        // fermer en cliquant à côté
        lightbox.addEventListener("click", (e) => {
        if (e.target === lightbox) {
            lightbox.style.display = "none";
        }
        });
    </script>
</body>
<footer>
    <div class="conteneur_footer" id="bottom">
        <div class="contact">
            <span><h4>Contact</h4></span>
            <span>adrienaxel.feraud@gmail.com</span>
            <span><img src="https://i59.servimg.com/u/f59/19/69/15/66/17485710.png"><a href="www.linkedin.com/in/adrien-feraud-b58447383" target="_blank"> LinkedIn</a></span>
            <span><img src="https://i59.servimg.com/u/f59/19/69/15/66/discor10.png"> Cosmofaee</span>
        </div>
        <div class="cv">
            <a href="index.html">CV</a>
            <span>Site par Adrien Feraud</span>
        </div>
    </div>
</footer>
</html>
