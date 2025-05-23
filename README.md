Voici un code HTML où se trouvent des erreurs d’accessibilité. Bien souvent les erreurs d’accessibilité sont des erreurs HTML . Vous pouvez utiliser une extension Web telle que Axe, Tanaguru ou Wave pour trouver une partie des erreurs.

<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8"/>
    <meta name="viewport" content="width=device-width"/>
    <link rel="stylesheet" href="index.css"/>
    <title>Atelier a11y Ada</title>
</head>
<body>
<div>
    <h1 class=block>Et Hop on test l'accessibilité de cette page</h1>
    <p>
        L'accessibilité est un concept fondamental qui vise à garantir que tous les individus, indépendamment de leurs
        capacités physiques ou cognitives, puissent accéder et utiliser de manière équitable les produits, les services,
        les environnements physiques et numériques, ainsi que les informations.
    <p>
        Dans un monde où la diversité est la norme, l'accessibilité est cruciale pour promouvoir l'inclusion et
        l'égalité des chances. Elle concerne tout un chacun, que ce soit les personnes en situation de handicap, les
        personnes âgées, les personnes malvoyantes ou malentendantes, ou encore celles ayant des difficultés
        d'apprentissage. L'accessibilité ne se limite pas seulement aux différences physiques, mais prend également en
        compte les diverses capacités, compétences, et contextes de chacun.
    </p>

    <p>
        Sur le plan physique, cela signifie que les espaces publics, les bâtiments, les transports, et autres
        infrastructures doivent être conçus de manière à être accessibles à tous. Cela implique, par exemple, la
        présence de rampes d'accès, d'ascenseurs, de signalisations adaptées, et de places de stationnement réservées.
    </p>
    <p>
        En ce qui concerne le numérique, l'accessibilité s'étend à l'ensemble des technologies, applications et sites
        web. Les contenus numériques doivent être structurés de manière claire, avec
        <a href="<https://accessibilite.numerique.gouv.fr/methode/criteres-et-tests/#3.2>">des couleurs contrastées</a>
        et une
        police lisible. Les vidéos doivent être sous-titrées pour les personnes sourdes ou malentendantes, et les
        interfaces doivent être utilisables au moyen d'une assistance technique telle que les lecteurs d'écran.
        L'accessibilité va au-delà de la simple conformité aux normes légales ou aux réglementations. C'est un état
        d'esprit qui vise à prendre en compte la diversité humaine dès la conception et à créer des environnements
        inclusifs dès le départ.
    </p>
    <p>
        En promouvant l'accessibilité, nous favorisons l'autonomie et l'inclusion sociale des personnes en situation de
        handicap, tout en améliorant l'expérience pour l'ensemble des utilisateurs. Cela peut aussi stimuler
        l'innovation, car les solutions accessibles exigent souvent de repenser les approches traditionnelles pour
        répondre aux besoins variés des utilisateurs.

    </p>

    <p>
        En fin de compte, l'accessibilité n'est pas simplement une option, mais un principe éthique et social qui nous
        appelle à créer un monde plus équitable, ouvert et inclusif pour tous. En nous efforçant de rendre notre
        société, notre technologie et notre environnement accessible à chacun, nous franchissons un pas important vers
        une société plus tolérante et bienveillante.
    </p>
    <div class="cards">
        <article class="card pb2">
            <header>
                <h2>Vraiment une dés plus belle ville de France ?</h2>
            </header>
            <img src="paris.jpg" alt="Tour eiffel">
            <div class="content">
                <p> Destination touristique visitée chaque année par quelque dix millions de touristes étrangers (treize
                    pour Paris et la petite couronne), Paris possède un patrimoine architectural mondialement connu
                    comme la cathédrale Notre-Dame de Paris, la tour Eiffel, le musée du Louvre ou encore l'Arc de
                    Triomphe. </p>
            </div>
            <div>
                <a class="button" href="<https://fr.wikipedia.org/wiki/Paris>">En savoir plus sur la ville de Paris</a>
            </div>
        </article>
        <article class="card pb2">
            <header>
                <h2>La plus belle ville de France</h2>
            </header>
            <img src="marseille.jpg" alt="Vue du vieux port de marseille et la bonne mère qui le surplombe">
            <div class="content">
                <p>Plus ancienne ville de France avec Béziers, fondée vers 600 av. J.-C. par des marins et des
                    marchands grecs originaires de Phocée sous le nom de
                    Massalía, Marseille est depuis l'Antiquité un important port de commerce et de passage.
                    Elle connaît un essor commercial considérable pendant la période coloniale et plus particulièrement
                    au cours du XIXe siècle, devenant une ville industrielle et négociante prospère5. </p>
            </div>
            <div>
                <a class="button" href="<https://fr.wikipedia.org/wiki/Marseille>">En savoir plus sur la ville de
                    Marseille</a>
            </div>
        </article>
        <article class="card pb2">
            <header>
                <h2>Nantes seconde plus belle ville de France</h2>
            </header>
            <img src="elephant.jpg" alt="">
            <div class="content">
                <p>Présentée comme « la ville la plus agréable d'Europe » par le magazine Time en 2004 et « meilleure
                    ville en France où travailler » par le site d'actualité The Local en 2018 et par le magazine
                    L'Express en 2017, Nantes reçoit le Prix de la Capitale verte de l’Europe en 2013 et le Prix de la
                    Capitale européenne de l'innovation en 2019.
                </p>
            </div>
            <div>
                <a class="button" href="<https://fr.wikipedia.org/wiki/Nantes>">En savoir plus sur la ville de Nantes</a>
            </div>
        </article>
    </div>
</div>
<div class="newletter pb2 flex">
    <form class="flex">
        <h4>
            Pour ne rien rater de notre classement des villes, inscrivez vous à notre newsletter
        </h4>
        <label for="username">Nom:<span aria-label="required">*</span></label>
        <input id="username" type="text" name="username" required/>

        <label for="name">Prénom:<span aria-label="required">*</span></label>
        <input id="name" type="text" name="name" required/>

        <label for="email">Email:<span aria-label="required">*</span></label>
        <input id="email" type="email" name="email" placeholder="nom@domaine.com" required/>

        <fieldset>
            <legend class="pt2">Choissisez ce qui vous interresse le plus dans notre newsletter</legend>

            <input type="radio" id="rank" name="rank"/>
            <label for="rank">Classement des villes</label><br/>

            <input type="radio" id="info" name="info"/>
            <label for="info">informations en temps reel des villes</label><br/>

            <input type="radio" id="news" name="news"/>
            <label for="news">Nouveautées des villes et villages de France</label>
        </fieldset>
        <button class="mgt2" type="submit">Valider votre inscription</button>
    </form>
</div>
</div>
<footer class="flex">
    <ul>
        <li class="pt2">
            <a href="<http://accessibilite.numerique.gouv.fr>">mentions légales</a>
        </li>
        <li class="pt2">
            <a href="">blog</a>
        </li>
    </ul>
</footer>
</body>
</html>