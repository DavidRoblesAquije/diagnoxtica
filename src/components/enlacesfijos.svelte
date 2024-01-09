<script>
    import facebook from "../images/icon facebook.png";
    import whatsapp from "../images/icon wsp.png";

    const enlaces = [
        {
            id: 1,
            name: "facebook",
            enlace: "https://www.facebook.com/diagnoxtica",
            icon: facebook,
            color: "#3b5998",
        },
        {
            id: 2,
            name: "whatsapp",
            enlace: "https://wa.me/992757093",
            icon: whatsapp,
            color: "#25D366",
        },
    ];
</script>

<div class="enlacesfijos">
    {#each enlaces as enlace (enlace.id)}
        <div class="enlace" style="background-color: {enlace.color}">
            <a href={enlace.enlace} target="_blank">
                <img src={enlace.icon} alt={enlace.name} />
            </a>
        </div>
    {/each}
</div>
