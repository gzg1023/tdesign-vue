<template>
  <div>
    <t-list :split="true" header="这里是 Header" footer="这里是 Footer">
      <t-list-item>
        <t-list-item-meta :image="imageUrl" title="列表标题" description="列表内容的描述性文字"></t-list-item-meta>
      </t-list-item>
      <t-list-item>
        <t-list-item-meta :image="imageUrl" title="列表标题" description="列表内容的描述性文字"></t-list-item-meta>
      </t-list-item>
      <t-list-item>
        <t-list-item-meta :image="imageUrl" title="列表标题" description="列表内容的描述性文字"></t-list-item-meta>
      </t-list-item>
    </t-list>

    <div style="margin-bottom:16px"></div>

    <t-list :split="true">
      <template #header>通过 Slot 插入的 Header</template>
      <t-list-item>
        <t-list-item-meta :image="imageUrl" title="列表标题" description="列表内容的描述性文字"></t-list-item-meta>
      </t-list-item>
      <t-list-item>
        <t-list-item-meta :image="imageUrl" title="列表标题" description="列表内容的描述性文字"></t-list-item-meta>
      </t-list-item>
      <t-list-item>
        <t-list-item-meta :image="imageUrl" title="列表标题" description="列表内容的描述性文字"></t-list-item-meta>
      </t-list-item>
      <template #footer>通过 Slot 插入的 Footer</template>
    </t-list>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imageUrl: 'https://tdesign.gtimg.com/site/avatar.jpg',
    };
  },
};
</script>
