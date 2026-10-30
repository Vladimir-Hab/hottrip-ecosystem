# HotTrip

Авиабилеты и горящие туры: портал, AI-бот, Telegram Mini App и автоматизированный канал. / Flights and hot tours: a portal, an AI bot, a Telegram Mini App and an automated channel.

**Сайт / Site:** https://hot-trip.ru/ · **Канал / Channel:** https://t.me/HotTripChat · **Mini App:** https://t.me/HotTripAppBot/app · **YouTube:** https://www.youtube.com/@hot-trip888

> В этом репозитории только описание проекта. Исходный код закрыт. / This repository contains the project description only; the source code is private.

## Что внутри / What it is

- **Портал:** поиск авиабилетов с городом вылета, лента горящих билетов из Telegram, курсы валют, журнал, направления, гайды, визы и страхование. AI-ассистент подбирает билеты и подписывает на снижение цены.
- **Бот и API:** Telegram-бот на LLM-агенте (OpenRouter, DeepSeek) с инструментами: поиск билетов, популярные направления, подписка на радар цен, определение города по геолокации. Данные из Travelpayouts API и собственного REST API на aiohttp.
- **Mini App:** каталог горящих билетов, поиск, радар цен, страхование и чек-лист путешественника внутри Telegram. Партнёрские ссылки идут через безопасный редирект со счётчиком кликов.
- **Фабрика контента:** каждые 2 часа n8n забирает предложения, сохраняет в PostgreSQL, собирает городские дайджесты, подбирает фото Pexels, рендерит видео через ffmpeg и публикует в автоматизированный канал.

Схема: Travelpayouts API → PostgreSQL → дайджесты → ffmpeg → каналы.

## Стек / Stack

Python · aiohttp · PostgreSQL · n8n · Telegram Bot API · LLM (OpenRouter, DeepSeek) · ffmpeg · SEO

## Автор / Author

Владимир Кальянов / Vladimir Kalianov — https://oneswitch.ru · [описание проекта](https://oneswitch.ru/raboty/hottrip/)
