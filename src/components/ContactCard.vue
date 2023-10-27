<script>
export default {
props: {
contact: { type: Object, required: true },
},
};
</script>
<template>
<div>
<div class="p-1">
<strong>Tên:gam </strong>
{{ contact.name }}
</div>
<div class="p-1">
<strong>E-mail:gamb1910512@student.ctu.edu.vn</strong>
{{ contact.email }}
</div>
<div class="p-1">
<strong>Địa chỉ:đại học cần thơ</strong>
{{ contact.address }}
</div>
<div class="p-1">
<strong>Điện thoại:0898016751</strong>
{{ contact.phone }}
</div>
<div class="p-1">
<strong>Liên hệ yêu thích:đọc sách&nbsp;</strong>
<i v-if="contact.favorite" class="fas fa-check"></i>
<i v-else class="fas fa-times"></i>
</div>
</div>
</template>