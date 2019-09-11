<template>
    <b-col md="6">
        <form class="">
            <div class="form-group">
                <font-awesome-icon icon="star" />
                <font-awesome-icon icon="star" />
                <font-awesome-icon icon="star" />
                <font-awesome-icon icon="star" />
                <font-awesome-icon icon="star" />
            </div>
            <div class="form-group"><textarea name="text" rows="3" placeholder="Type your reviews..."
                                              id="exampleForm.ControlTextarea1"
                                              class="form-control"></textarea></div>
            <button type="submit" class="btn btn-primary">Submit</button>
        </form>
        <h2 class="mt-5">Reviews</h2>
        <div class="reviews_list"></div>
    </b-col>
</template>

<script>
    export default {
        name: "Reviews"
    }
</script>

<style scoped>

</style>