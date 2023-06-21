<script>
    import img1 from '../../images/gallery-200819064756.jpg';
    import img2 from '../../images/gallery-200819064813.jpg';
    import img3 from '../../images/gallery-200819064829.jpg';
    import img4 from '../../images/gallery-200819064923.jpg';
    import img5 from '../../images/gallery-200930020210.jpg';
    import img6 from '../../images/FC-1.jpg';
    import img7 from '../../images/FC-2.jpg';

    let images = [
        img1,
        img2,
        img3,
        img4,
        img5,
        img6,
        img7
    ]
</script>

<div class="grid">
    {#each images as img}
 
        <img class="gallery-image" src={img} alt="gallery" />
  
    
    {/each}
  </div>

<style>
    .gallery-image{
        aspect-ratio: 16/9;
        border-radius: 30px;
        margin: 20px;
        border-radius: 30px;
      
    }
    .grid{
        display: block;
        
    }

</style>  