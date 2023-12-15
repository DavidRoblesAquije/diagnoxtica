<script>
    import bg1 from "../images/encabezado_bg1.png";
    import bg2 from "../images/encabezado_bg2.png";
    import bg3 from "../images/encabezado_bg3.png";
</script>

<header class="cabezera">
    <div
        id="carouselHeader"
        class="carousel slide h-100"
        data-ride="carousel"
        data-interval="10000"
        data-pause="false"
    >
        <div class="carousel-inner h-100">
            <div class="carousel-item firstCarousel h-100 active">
                <div class="carousel__container">
                    <div class="container">
                        <div class="carousel__presentation">
                            <h1 class="mb-3">DIAGNOXTICA</h1>
                            <p class="mb-4">
                                La sonrisa es uno de los elementos clave para la
                                armonia del rostro y la belleza
                            </p>
                            <button>Permitenos Presentarnos</button>
                        </div>
                    </div>
                </div>
                <!-- <img class="d-block" src={bg1} alt="First slide" /> -->
            </div>
            <div class="carousel-item secondCarousel h-100">
                <div class="carousel__container">
                    <div class="container">
                        <div class="carousel__presentation">
                            <h1>DIAGNOXTICA</h1>
                            <p>
                                La sonrisa es uno de los elementos clave para la
                                armonia del rostro y la belleza
                            </p>
                            <button>Permitenos Presentarnos</button>
                        </div>
                    </div>
                </div>
                <!-- <img class="d-block" src={bg2} alt="Second slide" /> -->
            </div>
            <div class="carousel-item thirdCarousel h-100">
                <div class="carousel__container">
                    <div class="container">
                        <div class="carousel__presentation">
                            <h1>DIAGNOXTICA</h1>
                            <p>
                                La sonrisa es uno de los elementos clave para la
                                armonia del rostro y la belleza
                            </p>
                            <button>Permitenos Presentarnos</button>
                        </div>
                    </div>
                </div>
                <!-- <img class="d-block" src={bg3} alt="Third slide" /> -->
            </div>
        </div>
        <a
            class="carousel-control-prev"
            href="#carouselHeader"
            role="button"
            data-slide="prev"
        >
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a
            class="carousel-control-next"
            href="#carouselHeader"
            role="button"
            data-slide="next"
        >
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
    </div>
</header>
