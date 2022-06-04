<template>
    <div class="nav">
        <div class="container">
            <div class="row">
                <div class="col-lg-5 col-md-7 col-12 py-5">
                    <div class="footer__nav row">
                        <div class="col-4">
                            <h3>dc comics</h3>
                            <ul class="p-0">
                                <li v-for="(link, index) in ComicsLinks" :key="index">
                                    <a :href="link.url">{{ link.title }}</a>
                                </li>
                            </ul>
                            <h3>shop</h3>
                            <ul class="p-0">
                                <li v-for="(link, index) in shopLinks" :key="index">
                                    <a :href="link.url">{{ link.title }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="col-4">
                            <h3>dc</h3>
                            <ul class="p-0">
                                <li v-for="(link, index) in DcLinks" :key="index">
                                    <a :href="link.url">{{ link.title }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="col-4">
                            <h3>sites</h3>
                            <ul class="p-0">
                                <li v-for="(link, index) in SitesLinks" :key="index">
                                    <a :href="link.url">{{ link.title }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "BaseFooterNav",
    data() {
        return {
            ComicsLinks: [
                {
                    title: "characters",
                    url: "#",
                },
                {
                    title: "comics",
                    url: "#",
                },
                {
                    title: "movies",
                    url: "#",
                },
                {
                    title: "TV",
                    url: "#",
                },
                {
                    title: "games",
                    url: "#",
                },
                {
                    title: "videos",
                    url: "#",
                },
                {
                    title: "news",
                    url: "#",
                },
            ],
            shopLinks: [
                {
                    title: "shop DC",
                    url: "#",
                },
                {
                    title: "shop DC collectibles",
                    url: "#",
                },
            ],
            DcLinks: [
                {
                    title: "terms of us",
                    url: "#",
                },
                {
                    title: "privacy policy (new)",
                    url: "#",
                },
                {
                    title: "ad choice",
                    url: "#",
                },
                {
                    title: "advertising",
                    url: "#",
                },
                {
                    title: "jobs",
                    url: "#",
                },
                {
                    title: "subscriptions",
                    url: "#",
                },
                {
                    title: "talent workshops",
                    url: "#",
                },
                {
                    title: "CPSC certificates",
                    url: "#",
                },
                {
                    title: "ratings",
                    url: "#",
                },
                {
                    title: "shop help",
                    url: "#",
                },
                {
                    title: "contact us",
                    url: "#",
                },
            ],
            SitesLinks: [
                {
                    title: "DC",
                    url: "#",
                },
                {
                    title: "MAD magazine",
                    url: "#",
                },
                {
                    title: "DC kids",
                    url: "#",
                },
                {
                    title: "DC universe",
                    url: "#",
                },
                {
                    title: "DC power visa",
                    url: "#",
                },
            ],
        };
    },
};
</script>

<style lang="scss" scoped>
.nav {
    background-image: url(../../assets/img/footer-bg.jpg);
    background-size: cover;

    .container {
        background-image: url(../../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;

        .row {
            width: 100%;

            .footer__nav {
                a {
                    color: var(--footer_link);
                    text-transform: capitalize;
                }
            }
        }
    }
}
</style>