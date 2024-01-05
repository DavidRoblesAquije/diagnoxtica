<script>
    import { each } from "svelte/internal";
    import serv1 from "../images/serv1.png";
    import serv2 from "../images/serv2.png";
    import serv3 from "../images/serv3.png";

    const services = [
        {
            id: 1,
            title: "Maxilofacial",
            image: serv1,
            description: "Descripcion del servicio 1",
        },
        {
            id: 2,
            title: "Radiografia",
            image: serv2,
            description: "Descripcion del servicio 2",
        },
        {
            id: 3,
            title: "Tomografía",
            image: serv3,
            description: "Descripcion del servicio 3",
        },
    ];
</script>

<section class="servicios__section">
    <div class="circleservicios"></div>

    <div class="container">
        <div class="row">
            <div class="col-12 d-flex justify-content-end">
                <div class="servicios__title">
                    <h2>Que te ofrecemos en</h2>
                    <h1>DIAGNOXTICA</h1>
                    <p>
                        En DIagnoxtica nos preocupamos por brindar los mejores
                        servicios para nuestros pacientes, Innovación y
                        tecnología en servicios para todas las áreas
                        odontológicas, con el acompañamiento de un staff
                        altamente especializado, accesible desde cualquier
                        ubicación.
                    </p>
                </div>
            </div>
        </div>

        <div class="servicios__cards mt-4">
            {#each services as service (service.id)}
                <div class="card servicios__card">
                    <img
                        class="card-img-top"
                        src={service.image}
                        alt={service.title}
                    />
                    <div class="card-body">
                        <h3 class="card-title">{service.title}</h3>
                        <p class="card-text">{service.description}</p>
                    </div>
                </div>
            {/each}
        </div>
    </div>
</section>
