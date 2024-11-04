<script>
  import SectionWrapper from "./SectionWrapper.svelte";

  let productFeatures = []

</script>
<SectionWrapper id="product">

    <div class="flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center pb-10 md:pb-14">
        <div class="flex flex-col gap-2 ">
            <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
                start your lifetime <span class="text-indigo-400">gym streak</span>
            </p>
            <h3 class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center">Features for everyone</h3>
        </div>
      
            {#each productFeatures as productFeature, index}
                <ProductCard productFeature={productFeature} index={index}>

                </ProductCard>
            {/each}
        

    </div>
</SectionWrapper>