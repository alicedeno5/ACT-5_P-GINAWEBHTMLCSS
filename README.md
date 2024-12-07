# ACT-5_P-GINAWEBHTMLCSS
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Actores Famosos</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- CSS Personalizado -->
    <style>
        /* Estilos Generales */
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to bottom, #e3f2fd, #ffffff);
            color: #343a40;
            margin-bottom: 100px;
        }

        /*Encabezado */
        header {
            background: linear-gradient(to right, #4a148c, #6a1b9a);
            color: white;
            text-align: center;
            padding: 30px 0;
            border-bottom: 5px solid #7e57c2;
        }

        header h1 {
            font-size: 2.8rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        header p {
            font-size: 1.2rem;
        }

        /* Tarjetas de Actores */
        .actor-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .actor-card:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
        }

        .actor-card img {
            width: 100%;
            max-width: 300px;
            height: 300px;
            object-fit: cover;
            border-radius: 10px;
            margin: auto;
            border: 3px solid #6a1b9a;
        }

        .actor-card h5 {
            margin-top: 10px;
            font-size: 1.25rem;
            color: #6a1b9a;
        }

        /* Modal Personalizado */
        .modal-header {
            background: linear-gradient(to right, #4a148c, #6a1b9a);
            color: white;
        }

        .modal-title {
            font-size: 1.5rem;
        }

        .modal-body img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            border: 3px solid #7e57c2;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }

        .modal-body p {
            font-size: 1rem;
            margin-top: 10px;
            color: #424242;
        }

        /* Footer */
        footer {
            background: #4a148c;
            color: white;
            text-align: center;
            padding: 15px 0;
            position: fixed;
            bottom: 0;
            width: 100%;
            border-top: 5px solid #7e57c2;
        }

        footer p {
            font-size: 0.9rem;
            margin: 0;
        }

        /* Botones */
        .btn-close {
            background-color: #6a1b9a;
        }

        .btn-close:hover {
            background-color: #4a148c;
        }
    </style>
</head>
<body>

    <!-- Encabezado -->
    <header class="text-center">
        <h1>Actores Famosos</h1>
        <p> Conoce a las figuras más emblemáticas de la historia del cine, cuyas actuaciones han dejado una huella imborrable en la industria cinematográfica.</p>
    </header>

    <!-- Galería de Actores -->
    <div class="container mt-5">
        <div class="row">
            <!-- Actor 1 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Leonardo_DiCaprio.jpg" class="img-fluid rounded" alt="Leonardo DiCaprio" data-bs-toggle="modal" data-bs-target="#actor1Modal">
                <h5 class="mt-3">Leonardo DiCaprio</h5>
            </div>
            <!-- Actor 2 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Denzel_Washington.jpg" class="img-fluid rounded" alt="Denzel Washington" data-bs-toggle="modal" data-bs-target="#actor2Modal">
                <h5 class="mt-3">Denzel Washington</h5>
            </div>
            <!-- Actor 3 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Morgan_Freeman.jpg" class="img-fluid rounded" alt="Morgan Freeman" data-bs-toggle="modal" data-bs-target="#actor3Modal">
                <h5 class="mt-3">Morgan Freeman</h5>
            </div>
        </div>
        <div class="row">
            <!-- Actor 4 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Tom_Hanks.jpg" class="img-fluid rounded" alt="Tom Hanks" data-bs-toggle="modal" data-bs-target="#actor4Modal">
                <h5 class="mt-3">Tom Hanks</h5>
            </div>
            <!-- Actor 5 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Will_Smith.jpg" class="img-fluid rounded" alt="Will Smith" data-bs-toggle="modal" data-bs-target="#actor5Modal">
                <h5 class="mt-3">Will Smith</h5>
            </div>
            <!-- Actor 6 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Angelina_Jolie.jpg" class="img-fluid rounded" alt="Angelina Jolie" data-bs-toggle="modal" data-bs-target="#actor6Modal">
                <h5 class="mt-3">Angelina Jolie</h5>
            </div>
        </div>
        <div class="row">
            <!-- Actor 7 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Julia_Roberts.jpg" class="img-fluid rounded" alt="Julia Roberts" data-bs-toggle="modal" data-bs-target="#actor7Modal">
                <h5 class="mt-3">Julia Roberts</h5>
            </div>
            <!-- Actor 8 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Meryl_Streep.jpg" class="img-fluid rounded" alt="Meryl Streep" data-bs-toggle="modal" data-bs-target="#actor8Modal">
                <h5 class="mt-3">Meryl Streep</h5>
            </div>
            <!-- Actor 9 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Nicole_Kidman.jpg" class="img-fluid rounded" alt="Nicole Kidman" data-bs-toggle="modal" data-bs-target="#actor9Modal">
                <h5 class="mt-3">Nicole Kidman</h5>
            </div>
        </div>
        <div class="row">
            <!-- Actor 10 -->
            <div class="col-md-4 mb-4 text-center actor-card">
                <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\Nicole_Kidman.jpg" class="img-fluid rounded" alt="Scarlett Johannsson" data-bs-toggle="modal" data-bs-target="#actor10Modal">
                <h5 class="mt-3">Scarlett Johannsson</h5>
            </div>
        </div>
    </div>

    <!-- Modales para Actores -->
    <!-- Modal Actor 1 -->
    <div class="modal fade" id="actor1Modal" tabindex="-1" aria-labelledby="actor1ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor1ModalLabel">Leonardo DiCaprio</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_LD.jpg" alt="Leonardo DiCaprio">
                    <p><strong>Biografía:</strong> Uno de los actores más destacados de Hollywood, conocido por su versatilidad en el cine.</p>
                    <p><strong>Películas destacadas:</strong> Titanic, El Lobo de Wall Street, Inception.</p>
                    <p><strong>Premios:</strong> Oscar por "The Revenant".</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 2 -->
    <div class="modal fade" id="actor2Modal" tabindex="-1" aria-labelledby="actor2ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor2ModalLabel">Denzel Washington</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_DW.jpg" alt="Denzel Washington">
                    <p><strong>Biografía:</strong> Reconocido por sus papeles intensos y poderosos en películas dramáticas.</p>
                    <p><strong>Películas destacadas:</strong> Training Day, Fences, Malcolm X.</p>
                    <p><strong>Premios:</strong> 2 Oscars y múltiples premios SAG.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 3 -->
    <div class="modal fade" id="actor3Modal" tabindex="-1" aria-labelledby="actor3ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor3ModalLabel">Morgan Freeman</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_MF.jpg" alt="Morgan Freeman">
                    <p><strong>Biografía:</strong> Conocido por su voz icónica y su habilidad para interpretar personajes sabios y entrañables.</p>
                    <p><strong>Películas destacadas:</strong> The Shawshank Redemption, Million Dollar Baby, Invictus.</p>
                    <p><strong>Premios:</strong> 1 Oscar, 1 Globo de Oro y múltiples reconocimientos honoríficos.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 4 -->
    <div class="modal fade" id="actor4Modal" tabindex="-1" aria-labelledby="actor4ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor4ModalLabel">Tom Hanks</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_TH.jpg" alt="Tom Hanks">
                    <p><strong>Biografía:</strong> Amado por su carisma y versatilidad, conocido por interpretar personajes entrañables en dramas y comedias.</p>
                    <p><strong>Películas destacadas:</strong>  Forrest Gump, Saving Private Ryan, Cast Away.</p>
                    <p><strong>Premios:</strong> 2 Oscars, 4 Globos de Oro y un premio Cecil B. DeMille.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 5 -->
    <div class="modal fade" id="actor5Modal" tabindex="-1" aria-labelledby="actor5ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor5ModalLabel">Will Smith</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_WS.jpg" alt="Will Smith">
                    <p><strong>Biografía:</strong> Destacado por su carisma y su capacidad para brillar tanto en comedias como en dramas.</p>
                    <p><strong>Películas destacadas:</strong> The Pursuit of Happyness, Men in Black, King Richard.</p>
                    <p><strong>Premios:</strong> 1 Oscar, 4 premios Grammy y múltiples nominaciones al Globo de Oro.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 6 -->
    <div class="modal fade" id="actor6Modal" tabindex="-1" aria-labelledby="actor6ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor6ModalLabel">Angelina Jolie</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_AJ.jpg" alt="Angelina Jolie">
                    <p><strong>Biografía:</strong> Conocida por su papel de Lara Croft y por su activismo humanitario.</p>
                    <p><strong>Películas destacadas:</strong> Maleficent, Girl, Interrupted, Tomb Raider.</p>
                    <p><strong>Premios:</strong> Oscar y múltiples premios de cine.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 7 -->
    <div class="modal fade" id="actor7Modal" tabindex="-1" aria-labelledby="actor7ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor7ModalLabel">Julia Roberts</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_JR.jpg" alt="Julia Roberts">
                    <p><strong>Biografía:</strong> Ícono de Hollywood, famosa por su sonrisa característica y su talento en comedias románticas y dramas.</p>
                    <p><strong>Películas destacadas:</strong> Pretty Woman, Erin Brockovich, Notting Hill.</p>
                    <p><strong>Premios:</strong> 1 Oscar, 3 Globos de Oro y múltiples premios del público.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 8 -->
    <div class="modal fade" id="actor8Modal" tabindex="-1" aria-labelledby="actor8ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor8ModalLabel">Meryl Streep</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_MS.jpg" alt="Meryl Streep">
                    <p><strong>Biografía:</strong> Considerada una de las mejores actrices de su generación por su capacidad camaleónica y su maestría en el arte de actuar.</p>
                    <p><strong>Películas destacadas:</strong>  The Devil Wears Prada, Sophie’s Choice, The Iron Lady.</p>
                    <p><strong>Premios:</strong> 3 Oscars, 9 Globos de Oro y un récord de nominaciones en la Academia.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 9 -->
    <div class="modal fade" id="actor9Modal" tabindex="-1" aria-labelledby="actor9ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor9ModalLabel">Nicole Kidman</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_NK.jpg" alt="Nicole Kidman">
                    <p><strong>Biografía:</strong> Reconocida por su elegancia y su habilidad para dar vida a personajes complejos en una variedad de géneros.</p>
                    <p><strong>Películas destacadas:</strong> Moulin Rouge!, The Hours, Big Little Lies (serie).</p>
                    <p><strong>Premios:</strong> 1 Oscar, 6 Globos de Oro y un premio Emmy.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Actor 10 -->
    <div class="modal fade" id="actor10Modal" tabindex="-1" aria-labelledby="actor10ModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="actor10ModalLabel">Scarlett Johannsson</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img src="C:\Users\Usuario\Desktop\IMÁGENES_VSC\ACTORES\PELÍCULAS\Pel_EJ.jpg" alt="Scarlett Johannsson">
                    <p><strong>Biografía:</strong> Admirada por su talento y presencia en pantalla, destacando tanto en películas de acción como en dramas profundos.</p>
                    <p><strong>Películas destacadas:</strong>  Lost in Translation, Marriage Story, Avengers: Endgame.</p>
                    <p><strong>Premios:</strong> 1 BAFTA, 1 Tony y múltiples nominaciones al Oscar y al Globo de Oro.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="text-center">
        <p>&copy; 2024 Actores Famosos | Todos los derechos reservados</p>
    </footer>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
