<script>
    import { each } from "svelte/internal";
    import comillas from "../images/comillas.png";

    let currentSlide = 0;
    const opinions = [
        {
            id: 1,
            name: "Dr. John Doe",
            comment:
                "Estoy muy satisfecho con el servicio de Diagnóstica. Su equipo profesional y amable hizo que mi experiencia con las radiografías fuera rápida y sin complicaciones. ¡Gracias por su eficiencia y atención excepcional",
        },
        {
            id: 2,
            name: "Dr. Jane Smith",
            comment:
                "Estoy muy satisfecho con el servicio de Diagnóstica. Su equipo profesional y amable hizo que mi experiencia con las radiografías fuera rápida y sin complicaciones.",
        },
        {
            id: 3,
            name: "Dr. Alice Johnson",
            comment:
                "Estoy muy satisfecho con el servicio de Diagnóstica. Su equipo profesional y amable hizo que",
        },
    ];

    function nextSlide() {
        currentSlide = (currentSlide + 1) % opinions.length;
    }

    function prevSlide() {
        currentSlide = (currentSlide - 1 + opinions.length) % opinions.length;
    }

    function changeSlide() {
        nextSlide();
    }

    setInterval(changeSlide, 4000);
</script>

<section class="opiniones__section">
    <div class="container">
        <div class="row">
            <div class="col-12 text-center">
                <div class="carousel mb-4">
                    <img class="comilla mb-3" src={comillas} alt="comillas" />
                    <div class="slide">
                        <p>{opinions[currentSlide].comment}</p>
                        <h3>{opinions[currentSlide].name}</h3>
                    </div>
                </div>

                {#each opinions as opinion (opinion.name)}
                    <div
                        class="dot dot{opinion.id} {currentSlide ===
                        opinion.id - 1
                            ? 'active'
                            : ''}"
                    >
                        <div class="dot__circle"></div>
                    </div>
                {/each}
            </div>
        </div>
    </div>
</section>
