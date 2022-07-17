<template>
<div class = "post">
    <div>
          <div><strong>Название:</strong> {{post.title}}</div>  
          <div><strong>Описание:</strong> {{post.body}}</div>
    
</div>
<post-item  
v-for="post in posts"
:post="post"
/>
       </div>


</template>

<script>
import PostItem from "@/components/PostItem";
export default {
components: {PostItem},
    props: {
        posts: {
            type: Array,
            required: true


        }
    }

}
</script>
        }
    }
}
<style scoped>
.post {
    padding: 15px;
    border: 2px solid teal;
    margin-top: 15px;
}

</style>