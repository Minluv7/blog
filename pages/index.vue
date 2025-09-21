<template>
    <div class="space">
        <Nav/>
        <main class="px-8 justify-items-center md:px-8 lg:px-16 xl :px-32 py-8">
            <div class="flex mt-4 flex-col md:flex-row gap-8 px-4 md:px-8 lg:px-16 py-8">
                <div class="md:w-1/2 w-full flex justify-center">
                    <img
                        src="/assets/image/theWay.jpg"
                        alt="The Way"
                        class=" object-cover shadow-md rounded-lg"/>
                </div>
                <div class="d:w-1/2 w-full space-y-4 text-justify">
                        <h1 class="text-center md:text-left text-xl md:text-3xl font-semibold uppercase text-[#013A63]">
                            Beyaz tavşanı takip et; o seni, varman gereken yere götürür.
                        </h1>
            
                        <p>“İki günlük dünya” dediler, öyle değil mi?
                        Zaman denen şey nedir aslında?
                        Ve ben kimim bu döngüde?
                        Amacım ne? Neden buradayım? Görevim ne?</p>

                        <p>Bu kadar karmaşanın sebebi ne?
                        Ben mi kafayı yedim, yoksa sistem mi beni buna zorluyor?
                        Gerçekten özgürce mi düşünüyoruz biz?
                        Yoksa fark etmeden manipüle mi ediliyoruz?</p>

                        <p>Belki de ben aslında yokum.
                        Sen de yoksun.
                        Hiçbir şey gerçekten “var” değil.
                        Buradaki her şey bilinçaltımın bir yansıması olabilir.</p>

                        <p>Her şeyi anlamak için başa mı dönelim? Hani bir patlama (Big Bang) olmuştu ya... Atomlar, parçacıklar, enerji, yıldızlar, galaksiler, evren... 
                        ve en son biz, insanlar...</p>

                        <p>Bir dakika, bir dakika... Zamanı geriye alabilir miyiz? Yoksa geçmişi boş verip ileriye mi bakmalıyız? Ya geçmiş bize hâlâ bir şey anlatıyorsa? </p>

                        <p>Ademoğlu neden yaratıldı?
                            Âlem mi Adem’de saklı, yoksa Adem mi âlemde?
                        </p>
                        <p>
                            Peki, neden "ölmeden önce ölmek" gerek? Bunu nasıl mümkün kılabiliriz?
                        </p>
                        <p>Hiç olmakta başlar her şey.
                        Çünkü hiçlik, her şeyin başlangıcıdır.</p>
                        <p><em>- Nese</em></p>
                </div>
               
            </div>
            <div>
                <NuxtLink
                    to="/blog"
                    class="bg-[#013A63] text-white px-6 py-3 rounded-lg text-center hover:bg-[#012a4a] transition duration-300">
                    Blog sayfasına git
                </NuxtLink>
            </div>
            
        </main>
    </div>
</template>

<script lang="ts" setup>

</script>

<style scoped>

</style>