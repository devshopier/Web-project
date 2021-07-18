# Création de Pages Web Accessibles

! [Tout sur l'accessibilité](/sketchnotes/webdev101-a11y.png)
> SketchNote par[Tomomi Imura](https://twitter.com/girlie_mac)

## Quiz préalable
[Quiz préalable](https://nice-beach-0fe9e9d0f.azurestaticapps.net/quiz/5)

> La puissance du Web est dans son universalité.L'accès par tout le monde indépendamment d'invalidité est un aspect essentiel.
>
> \- Sir Timothy Berners-Lee, directeur du W3C et inventeur du World Wide Web

Cette citation met parfaitement l'accent sur l'importance de créer des sites Web accessibles.Une application qui ne peut pas être accessible par tous est par définition exclusionnaire.En tant que développeurs Web, nous devrions toujours avoir l'accessibilité à l'esprit.En ayant cet objectif dès le début, vous serez déjà bien lancé sur la façon de vous assurer que tout le monde peut accéder aux pages que vous créez. Dans cette leçon, vous découvrirez les outils pouvant vous aider à vous assurer que vos éléments Web sont accessibles et comment développer avec l'accessibilité à l'esprit. 

> Vous pouvez accéder à cette leçon sur [Microsoft Learn](https://docs.microsoft.com/learn/modules/web-development-101/accessibility?WT.mc_id=academic-13441-cxa)!

## Outils à utiliser

### Lecteurs d'écran (Screen readers)

L'un des outils d'accessibilité les plus connus sont les lecteurs d'écran.

[Les lecteurs d'écran](https://en.wikipedia.org/wiki/Screen_reader) sont des clients couramment utilisés pour ceux qui ont des déficiences visuelles. De la même manière que nous passons du temps à nous assurer qu'un navigateur transmette correctement les informations que nous souhaitons partager, nous devons également le faire pour un lecteur d'écran.

À la base, un lecteur d'écran lira une page de haut en bas de manière audible. Si votre page ne contient que du texte, le lecteur transmettra les informations de la même manière qu'un navigateur. Bien sûr, les pages Web sont rarement purement textuelles ; elles contiendront des liens, des graphiques, des couleurs et d'autres composants visuels. Il faut veiller à ce que ces informations soient lues correctement par un lecteur d'écran.

Chaque développeur Web doit se familiariser avec un lecteur d'écran. Comme souligné ci-dessus, c'est le client que vos utilisateurs utiliseront. De la même manière que vous connaissez le fonctionnement d'un navigateur, vous devez apprendre comment fonctionne un lecteur d'écran. Heureusement, les lecteurs d'écran sont intégrés à la plupart des systèmes d'exploitation.

Certains navigateurs disposent également d'outils et d'extensions intégrés qui peuvent lire le texte à voix haute ou même fournir des fonctionnalités de navigation de base, telles que [ces outils de navigateur Edge axés sur l'accessibilité](https://support.microsoft.com/help/4000734/microsoft-edge-accessibility-features). Ce sont également des outils d'accessibilité importants, mais ils fonctionnent très différemment des lecteurs d'écran et ils ne doivent pas être confondus avec des outils de test de lecteurs d'écran.

✅ Essayez un lecteur d'écran et un lecteur de texte de navigateur. Sous Windows, [Narrateur](https://support.microsoft.com/windows/complete-guide-to-narrator-e4397a0d-ef4f-b386-d8ae-c172f109bdb1) est inclus par défaut, et [JAWS](https:// webaim.org/articles/jaws/) et [NVDA](https://www.nvaccess.org/about-nvda/) peuvent également être installés. Sur macOS et iOS, [VoiceOver](https://support.apple.com/guide/voiceover/welcome/10) est installé par défaut.

### Zoom

Un autre outil couramment utilisé par les personnes malvoyantes est le zoom. Le type de zoom le plus basique est le zoom statique, contrôlé par `Ctrl + signe plus (+)` ou en diminuant la résolution de l'écran. Ce type de zoom entraîne le redimensionnement de la page entière, il est donc important d'utiliser un [design responsive](https://developer.mozilla.org/docs/Learn/CSS/CSS_layout/Responsive_Design) pour offrir une bonne expérience utilisateur à des niveaux de zoom accrus .

Un autre type de zoom repose sur un logiciel spécialisé pour agrandir une zone de l'écran et effectuer un panoramique, un peu comme avec une vraie loupe. Sous Windows, [Loupe](https://support.microsoft.com/windows/use-magnifier-to-make-things-on-the-screen-easier-to-see-414948ba-8b1c-d3bd-8615-0e5e32204198 ) est intégré, et [ZoomText](https://www.freedomscientific.com/training/zoomtext/getting-started/) est un logiciel de grossissement tiers avec plus de fonctionnalités et une plus grande base d'utilisateurs. MacOS et iOS ont tous deux un logiciel de grossissement intégré appelé [Zoom](https://www.apple.com/accessibility/mac/vision/).

### Contrôleurs de contraste

Les couleurs sur les sites Web doivent être soigneusement choisies pour répondre aux besoins des utilisateurs daltoniens ou des personnes qui ont des difficultés à voir les couleurs à faible contraste.

✅ Testez un site Web que vous aimez utiliser pour l'utilisation des couleurs avec une extension de navigateur telle que [le vérificateur de couleurs de WCAG](https://microsoftedge.microsoft.com/addons/detail/wcag-color-contrast-check/idahaggnlnekelhgplklhfpchbfdmkjp?hl=en-US). Qu'apprenez-vous?

### Lighthouse

Dans la zone des outils de développement de votre navigateur, vous trouverez l'outil Lighthouse. Cet outil est important pour obtenir une première vue de l'accessibilité (ainsi que d'autres analyses) d'un site Web. Bien qu'il soit important de ne pas se fier exclusivement à Lighthouse, un score de 100 % est très utile comme référence.

✅ Trouvez Lighthouse dans le panneau des outils de développement de votre navigateur et lancez une analyse sur n'importe quel site. Que découvrez vous ?

## Concevoir pour l'accessibilité

L'accessibilité est un sujet relativement vaste. Pour vous aider, de nombreuses ressources sont disponibles.

- [Accessible U - Université du Minnesota](https://accessibility.umn.edu/your-role/web-developers)

Bien que nous ne puissions pas couvrir tous les aspects de la création de sites accessibles, vous trouverez ci-dessous quelques-uns des principes fondamentaux que vous voudrez mettre en œuvre. Concevoir une page accessible dès le départ est **toujours** plus facile que de revenir à une page existante pour la rendre accessible.

## Bons principes d'affichage

### Palettes de couleurs sûres

Les gens voient le monde de différentes manières, et cela inclut les couleurs. Lorsque vous sélectionnez un schéma de couleurs pour votre site, vous devez vous assurer qu'il est accessible à tous. Un excellent [outil pour générer des palettes de couleurs est Color Safe](http://colorsafe.co/).

✅ Identifiez un site Web qui est très problématique dans son utilisation de la couleur. Pourquoi?

### Utilisez le bon code HTML

Avec CSS et JavaScript, il est possible de faire ressembler n'importe quel élément à n'importe quel type de contrôle. `<span>` pourrait être utilisé pour créer un `<button>`, et `<b>` pourrait devenir un hyperlien. Bien que cela puisse être considéré comme plus facile à styliser, cela ne transmet rien à un lecteur d'écran. Utilisez le code HTML approprié lors de la création de contrôles sur une page. Si vous voulez un lien hypertexte, utilisez `<a>`. Utiliser le bon code HTML pour le bon contrôle s'appelle utiliser le HTML sémantique.

✅ Allez sur n'importe quel site Web et voyez si les concepteurs et les développeurs utilisent correctement le HTML. Pouvez-vous trouver un bouton qui devrait être un lien ? Astuce : faites un clic droit et choisissez « Afficher la source de la page » dans votre navigateur pour consulter le code sous-jacent.

### Créer une hiérarchie d'en-têtes descriptive

Les utilisateurs de lecteurs d'écran [se fient fortement aux titres](https://webaim.org/projects/screenreadersurvey8/#finding) pour trouver des informations et parcourir une page. La rédaction d'un contenu de titre descriptif et l'utilisation de balises de titre sémantique sont importantes pour créer un site facilement navigable pour les utilisateurs de lecteurs d'écran.

### Utilisez de bons indices visuels

CSS offre un contrôle complet sur l'apparence de n'importe quel élément d'une page. Vous pouvez créer des zones de texte sans contour ou des liens hypertexte sans soulignement. Malheureusement, la suppression de ces indices peut rendre plus difficile, pour quelqu'un qui en dépend, la capacité de reconnaître le type de contrôle.

## L'importance du texte de lien

Les hyperliens sont essentiels à la navigation sur le Web. Par conséquent, s'assurer qu'un lecteur d'écran peut lire correctement les liens permet à tous les utilisateurs de naviguer sur votre site.

### Lecteurs d'écran et liens

Comme on peut s'y attendre, les lecteurs d'écran lisent le texte de lien de la même manière qu'ils liraient n'importe quel autre texte de la page. Dans cet esprit, le texte présenté ci-dessous peut sembler parfaitement acceptable.

> Le petit pingouin, parfois appelé pingouin fée, est le plus petit pingouin du monde. [Cliquez ici](https://en.wikipedia.org/wiki/Little_penguin) pour plus d'informations.

> Le petit pingouin, parfois appelé pingouin fée, est le plus petit pingouin du monde. Visitez https://en.wikipedia.org/wiki/Little_penguin pour plus d'informations.

> **REMARQUE** Au moment où vous êtes sur le point de lire, vous ne devez **jamais** créer des liens qui ressemblent à ceux ci-dessus.

N'oubliez pas que les lecteurs d'écran sont une interface différente des navigateurs avec un ensemble de fonctionnalités différent.

### Le problème avec l'utilisation de l'URL

Les lecteurs d'écran lisent le texte. Si une URL apparaît dans le texte, le lecteur d'écran lira l'URL. De manière générale, l'URL ne transmet pas d'informations significatives et peut sembler ennuyeuse. Vous avez peut-être vécu cela si votre téléphone a déjà lu de manière audible un message texte avec une URL.

### Le problème avec "cliquez ici"

Les lecteurs d'écran ont également la possibilité de lire uniquement les hyperliens sur une page, de la même manière qu'une personne voyante numériserait une page à la recherche de liens. Si le texte du lien est toujours « cliquez ici », tout ce que l'utilisateur entendra est « cliquez ici, cliquez ici, cliquez ici, cliquez ici, cliquez ici, ... » Tous les liens sont désormais indiscernables les uns des autres.

### Bon texte de lien

Un bon texte de lien décrit brièvement ce qui se trouve de l'autre côté du lien. Dans l'exemple ci-dessus parlant de petits pingouins, le lien renvoie à la page Wikipedia sur l'espèce. L'expression *petits pingouins* constituerait un texte de lien parfait car elle indique clairement ce que quelqu'un apprendra s'il clique sur le lien - petits pingouins.

> Le [petit pingouin](https://en.wikipedia.org/wiki/Little_penguin), parfois appelé pingouin féerique, est le plus petit pingouin du monde.

✅ Surfez sur le Web pendant quelques minutes pour trouver des pages qui utilisent des stratégies de liens obscures. Comparez-les avec d'autres sites mieux liés. Qu'apprenez-vous?

#### Notes du moteur de recherche

En plus de garantir que votre site est accessible à tous, vous aiderez également les moteurs de recherche à naviguer sur votre site. Les moteurs de recherche utilisent le texte du lien pour apprendre les sujets des pages. Donc, utiliser un bon texte de lien aide tout le monde !

### ARIA

Imaginez la page suivante :

| Produit      | Description        | Commande        |
| ------------ | ------------------ | ------------ |
| Widget       | [Description]('#') | [Commande]('#') |
| Super widget | [Description]('#') | [Commande]('#') |

In this example, duplicating the text of description and order make sense for someone using a browser. However, someone using a screen reader would only hear the words *description* and *order* repeated without context.

To support these types of scenarios, HTML supports a set of attributes known as [Accessible Rich Internet Applications (ARIA)](https://developer.mozilla.org/docs/Web/Accessibility/ARIA). These attributes allow you to provide additional information to screen readers.

> **NOTE**: Like many aspects of HTML, browser and screen reader support may vary. However, most mainline clients support ARIA attributes.

You can use `aria-label` to describe the link when the format of the page doesn't allow you to. The description for widget could be set as

``` html
<a href="#" aria-label="Widget description">description</a>
```

✅ In general, using Semantic markup as described above supersedes the use of ARIA, but sometimes there is no semantic equivalent for various HTML widgets. A good example is a Tree. There's no HTML equivalent for a tree, so you identify the generic `<div>` for this element with a proper role and aria values. The [MDN documentation on ARIA](https://developer.mozilla.org/docs/Web/Accessibility/ARIA) contains more useful information.

```html
<h2 id="tree-label">File Viewer</h2>
<div role="tree" aria-labelledby="tree-label">
  <div role="treeitem" aria-expanded="false" tabindex="0">Uploads</div>
</div>
```

## Images

It goes without saying screen readers are unable to automatically read what's in an image. Ensuring images are accessible doesn't take much work - it's what the `alt` attribute is all about. All meaningful images should have an `alt` to describe what they are.
Images that are purely decorative should have their `alt` attribute set to an empty string: `alt=""`. This prevents screen readers from unnecessarily announcing the decorative image.

✅ As you might expect, search engines are also unable to understand what's in an image. They also use alt text. So once again, ensuring your page is accessible provides additional bonuses!

## The keyboard

Some users are unable to use a mouse or trackpad, instead relying on keyboard interactions to tab from one element to the next. It's important for your web site to present your content in logical order so a keyboard user can access each interactive element as they move down a document. If you build your web pages with semantic markup and use CSS to style their visual layout, your site should be keyboard-navigable, but it's important to test this aspect manually. Learn more about [keyboard navigation strategies](https://webaim.org/techniques/keyboard/).

✅ Go to any web site and try to navigate through it using only your keyboard. What works, what doesn't work? Why?

## Summary

A web accessible to some is not a truly 'world-wide web'. The best way to ensure the sites you create are accessible is to incorporate accessibility best practices from the start. While there are extra steps involved, incorporating these skills into your workflow now will mean all pages you create will be accessible.

---

## 🚀 Challenge

Take this HTML and rewrite it to be as accessible as possible, given the strategies you learned.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>
      Example
    </title>
    <link href='../assets/style.css' rel='stylesheet' type='text/css'>
  </head>
  <body>
    <div class="site-header">
      <p class="site-title">Turtle Ipsum</p>
      <p class="site-subtitle">The World's Premier Turtle Fan Club</p>
    </div>
    <div class="main-nav">
      <p class="nav-header">Resources</p>
      <div class="nav-list">
        <p class="nav-item nav-item-bull"><a href="https://www.youtube.com/watch?v=CMNry4PE93Y">"I like turtles"</a></p>
        <p class="nav-item nav-item-bull"><a href="https://en.wikipedia.org/wiki/Turtle">Basic Turtle Info</a></p>
        <p class="nav-item nav-item-bull"><a href="https://en.wikipedia.org/wiki/Turtles_(chocolate)">Chocolate Turtles</a></p>
      </div>
    </div>
    <div class="main-content">
      <div>
        <p class="page-title">Welcome to Turtle Ipsum. 
            <a href="">Click here</a> to learn more.
        </p>
        <p class="article-text">
          Turtle ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum
        </p>
      </div>
    </div>
    <div class="footer">
      <div class="footer-section">
        <span class="button">Sign up for turtle news</span>
      </div><div class="footer-section">
        <p class="nav-header footer-title">
          Internal Pages
        </p>
        <div class="nav-list">
          <p class="nav-item nav-item-bull"><a href="../">Index</a></p>
          <p class="nav-item nav-item-bull"><a href="../semantic">Semantic Example</a></p>
        </div>
      </div>
      <p class="footer-copyright">&copy; 2016 Instrument</span>
    </div>
  </body>
</html>
```

## Quiz de validation des connaissances
[Quiz de validation des connaissances](https://nice-beach-0fe9e9d0f.azurestaticapps.net/quiz/6)

## Review & Self Study

Many governments have laws regarding accessibility requirements. Read up on your home country's accessibility laws. What is covered, and what isn't? An example is [this government web site](https://accessibility.blog.gov.uk/).

## Assignment
 
[Analyze a non-accessible web site](assignment.md)

Credits: [Turtle Ipsum](https://github.com/Instrument/semantic-html-sample) by Instrument
