<template>
  <MDBCard class="mb-3 w-100 overflow-hidden">
    <img
      src="https://cdn2.oceansbridge.com/2019/05/25024700/The-Storyteller-Eugenio-Zampighi-Oil-Painting-1.jpg"
      class="position-absolute w-100 h-100"
      style="object-fit: cover; opacity: 0.13"
      alt="bg"
    />
    <MDBRow class="g-0 position-relative" style="z-index: 5">
      <MDBCol md="3">
        <MDBCardImg :src="img_url" style="height: 300px; border-radius: 0" />
      </MDBCol>
      <MDBCol md="8">
        <MDBCardBody class="d-flex flex-column h-100">
          <div class="category-title mb-3">
            <small class="text-info"
              ><i class="fas fa-book-open fa-sm me-2"></i>Short Story</small
            >
          </div>
          <h3>เจอคุณครั้งแรก</h3>
          <MDBCardText class="article-preview">
            "ผมเห็นคุณแล้ว กำลังกินเบียร์อยู่"
            ไลน์ในโทรศัพท์ของฉันเด้งขึ้นมาแสดงข้อความ ข้อความหนึ่ง
            มันทำให้ฉันรู้สึกอายนิดหน่อย การเจอกันครั้งแรกของเราสองคน
            ควรจะน่าประทับใจกว่านี้ไหมนะ
            "แล้วคุณจะมาหาเรามั้ย"เพราะมีปริมาณแอลกอฮอล์ในเลือดหรือป่าวนะ
            ฉันถึงกล้าคิดกล้าทำมากขนาดนี้
          </MDBCardText>
          <div class="mt-auto">
            <MDBCardText>
              <small class="text-muted d-block">
                <i class="fas fa-pen-nib me-2"></i>Codename_T
              </small>
              <small class="text-muted">
                <i class="fas fa-calendar-day me-2"></i>Time
              </small>
            </MDBCardText>
          </div>
        </MDBCardBody>
      </MDBCol>
    </MDBRow>
  </MDBCard>
</template>
<script setup>
import { ref } from "vue";
import {
  MDBCardBody,
  MDBCardText,
  MDBRow,
  MDBCol,
  MDBCardImg,
  MDBCard,
} from "mdb-vue-ui-kit";
import ContentCardbg from "@/assets/card_covers/mayastepien_habits_meal.jpg";
const img_url = ref(
  "https://images.saatchiart.com/saatchi/1652254/art/7905214/6972892-HSC00001-7.jpg"
);
</script>
<style scoped>
img.side-card-img {
  height: 600px !important;
  object-fit: cover;
}
.article-preview {
  font-weight: 300;
  font-size: 11pt;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 2; /* number of lines to show */
  line-clamp: 2;
  -webkit-box-orient: vertical;
}
</style>
