🔌 EzHitboxes
Хитбоксы в Minecraft 1.16.5

⚡ Как настроить?
Изменить размер
Радужный водяной знак (его можно отключить)
Легко настроить
Привязки:
I - Отключить водяной знак
K - Увеличить размер хитбоксов
J - Уменьшить размер хитбоксов

Учебник: Нажмите (на русском языке)

❓ Как это работает?
    public void onUpdate(RenderPlayerEvent e) {
        Entity player = e.getEntity();
        
        if (player != Minecraft.getInstance().player) {
            player.setBoundingBox(new AxisAlignedBB(
                            player.getX() - size,
                            player.getBoundingBox().minY,
                            player.getZ() - size,
                            player.getX() + size,
                            player.getBoundingBox().maxY,
                            player.getZ() + size
                    )
            );
        }
    }
📱 Скриншоты
<img width="437" height="639" alt="image" src="https://github.com/user-attachments/assets/b08372ba-546a-4f89-8866-4e832dd0ae66" />
