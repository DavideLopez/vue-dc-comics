<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="DClogo">
            </div>
            <nav class="nav">
                <ul class="nav-list">
                    <li v-for="(link, index) in links" :key="index" class="nav-item">
                        <a class="nav-link" href="link.href">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>


<script>

    const links = [
        {
            text: 'characters',
            href: '#',
            active: true
        },
        {
            text: 'comics',
            href: '#',
            active: true
        },
        {
            text: 'movies',
            href: '#',
            active: true
        },
        {
            text: 'TV',
            href: '#',
            active: true
        },
        {
            text: 'games',
            href: '#',
            active: true
        },
        {
            text: 'collectibles',
            href: '#',
            active: true
        },
        {
            text: 'video',
            href: '#',
            active: true
        },
        {
            text: 'fans',
            href: '#',
            active: true
        },
        {
            text: 'news',
            href: '#',
            active: true
        },
        {
            text: 'shop',
            href: '#',
            active: true
        },
    ]

    export default {
        data() {
            return {
                links: links
            }
        }

    }
</script>

<style lang="scss" scoped>
    header {
        padding: 1rem 0;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            width: 80px;
            height: 80px;

            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
            }
        }

        .nav {
            .nav-list {
                display: flex;
                align-items: center;
                font-weight: bold;
                font-size: 14px;
            }

            .nav-link:hover {
                border-bottom: 5px solid #0282f9;
            }
            
            .nav-link {
                padding: 0 12px;
                line-height: 1.5rem;
                text-transform: uppercase;
            }
        }
    }
   

</style>