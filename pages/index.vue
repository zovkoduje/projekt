<template>
    
    <div class="bg-gradient-to-br from-blue-200 to-white  pb-10">
        <Navigation/>
        <div class="flex flex-col md:flex-row items-center m-36">
            <div class="relative z-10 order-1 md:order-1">
                <h1 class="text-gray-700 font-black text-9xl">Let's change the future</h1>
                <btn class="mt-10"/>
            </div>
            <Cover class="order-2 md:order-2"/>
        </div>

        <div>
            <Carousel/>
        </div>

    </div>
    <div class="relative bg-gradient-to-t from-sky-600 to-sky-900 flex items-center h-screen">
        <img src="https://s3-alpha-sig.figma.com/img/0b39/c524/967231efbba0cc2c88761eabdf55b07e?Expires=1685318400&Signature=P9OaqsHMH6FMCPJ0x1MofK~A3IqXaAE0WaDGx4nhp2L1pur4Yc6oz2~Rg613Lke0vsSopGj0Nsji9-HujOtFhrgMuZ9-AFJBjuUJtkKqavX0-Bir7KybJHhsScn2RE-j4LSzMSAKN-9WjOIGfkaXBUzonxUnqomTeFxKnGtsm3Uud03BHmvzOst0xhAtTG3HIfLVosdyMn8iWPi~oUoc5wI~2VEQuGbL~ZS9gg3RVZpInVwgfd-Df-eaNHgSPKuzLcqvSVlxkxaX3ziLwl44Op3LSYxoOHzAf34eVvV1I0TE~265b78eNG4zJd3jaE-sRHn8Pjm4wRYuOtTPT8uBeQ__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4"
        class="w-full h-full object-cover absolute mix-blend-overlay opacity-5">
        <img class="absolute top-0 right-0" src="/imgs/Vector_31.png">
                    
        <div class="relative w-1/2">
                <img class="absolute -left-56 @screen md:left-1/4 bottom-1/2" src="/imgs/Vector_35.png">
                <img class="absolute mt-28 -right-32" src="/imgs/Vector_48.png">
                <img class="hidden @screen md:flex left-16 mt-60 z-10 absolute" src="/imgs/Vector_28.png">
                <img class="hidden md:flex absolute left-5 top-96 pt-96 z-10 " src="/imgs/Vector_54.svg">
            </div>
        <Quote/>        
    </div>
    <Worldmap></Worldmap>
    <WordlmapMobile></WordlmapMobile>
    <div class=" relative bg-[#F1F1F1]">
        <Horizontal text="SPECIFICATION"/>
        <Vertical text="SPECIFICATION" color="text-white"/>
        <div>
        <Content
        title="Discovery process"
        textContent="Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, sunt totam? Praesentium, accusantium, nam esse quo tenetur, fuga quisquam blanditiis excepturi adipisci animi asperiores laudantium perferendis doloremque id! Quia, autem."
        image-src="/imgs/Vector_17.png"
        :image-on-left="true"
        />
        </div>


    </div>
    <div class="bg-gradient-to-tr from-gray-400 to-gray-700 flex-row">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#f1f1f1" fill-opacity="1" d="M0,192L30,208C60,224,120,256,180,240C240,224,300,160,360,138.7C420,117,480,139,540,138.7C600,139,660,117,720,138.7C780,160,840,224,900,250.7C960,277,1020,267,1080,245.3C1140,224,1200,192,1260,202.7C1320,213,1380,267,1410,293.3L1440,320L1440,0L1410,0C1380,0,1320,0,1260,0C1200,0,1140,0,1080,0C1020,0,960,0,900,0C840,0,780,0,720,0C660,0,600,0,540,0C480,0,420,0,360,0C300,0,240,0,180,0C120,0,60,0,30,0L0,0Z"></path></svg>
        <Content
            title="Feature breakdown"
            textContent="Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, sunt totam? Praesentium, accusantium, nam esse quo tenetur, fuga quisquam blanditiis excepturi adipisci animi asperiores laudantium perferendis doloremque id! Quia, autem."
            image-src="/imgs/Vector_18.png"
            :image-on-left="false"
            textColor="white"
            
            />
        
    </div>
    <div class="bg-[#F1F1F1] h-screen flex relative justify-between pt-32">
        <Content
            title="Technical analyst"
            textContent="Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, sunt totam? Praesentium, accusantium, nam esse quo tenetur, fuga quisquam blanditiis excepturi adipisci animi asperiores laudantium perferendis doloremque id! Quia, autem."
            image-src="/imgs/Vector_11.png"
            :image-on-left="true"
            
            />
    </div>
    <div class="bg-gradient-to-t from-[#34bbd9] to-[#2f4e7b] flex-row pt-10 relative">
        <Horizontal text="ESTIMATION " color="text-white" backgroundColor="white"/>
        <Vertical text="ESTIMATION"/>        
        <Content
            title="Estimation summary"
            textContent="Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, sunt totam? Praesentium, accusantium, nam esse quo tenetur, fuga quisquam blanditiis excepturi adipisci animi asperiores laudantium perferendis doloremque id! Quia, autem."
            image-src="/imgs/Vector_34.png"
            :image-on-left="false"
            textColor="white"
            
            />
        <Content
            title="Cost optimisation"
            textContent="Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, sunt totam? Praesentium, accusantium, nam esse quo tenetur, fuga quisquam blanditiis excepturi adipisci animi asperiores laudantium perferendis doloremque id! Quia, autem."
            image-src="/imgs/Vector_171.png"
            :image-on-left="true"
            textColor="white"
            
            />
        
            
    </div>
    <div class="relative flex-row justify-between pt-32 bg-gradient-to-t from-white to-blue-100">
        <svg class="-mt-32" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#34bbd9" fill-opacity="1" d="M0,224L48,229.3C96,235,192,245,288,256C384,267,480,277,576,277.3C672,277,768,267,864,256C960,245,1056,235,1152,202.7C1248,171,1344,117,1392,90.7L1440,
            64L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"></path></svg>
        <Horizontal text="REALISATION "/>
        <Vertical text="REALISATION"/>
        <Content
            title="Team assembling"
            textContent="Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, sunt totam? Praesentium, accusantium, nam esse quo tenetur, fuga quisquam blanditiis excepturi adipisci animi asperiores laudantium perferendis doloremque id! Quia, autem."
            image-src="/imgs/Vector_10.png"
            :image-on-left="false"
            
            />
        <Content
            title="Tech leadership"
            textContent="Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, sunt totam? Praesentium, accusantium, nam esse quo tenetur, fuga quisquam blanditiis excepturi adipisci animi asperiores laudantium perferendis doloremque id! Quia, autem."
            image-src="/imgs/Vector_7.png"
            :image-on-left="true"
            
            />
    </div>    
    <div class="pt-32 pb-10 bg-[url('/imgs/Contact_form_background.png')] bg-no-repeat bg-cover justify-center">
        
            <Contact></Contact>
    </div>   
</template>
<script>


</script>