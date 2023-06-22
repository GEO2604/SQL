#first I created a makeup store database, then displayed the database ordered by price, by year product lauched, and by items best to least sold.

CREATE TABLE makeup (id INTEGER PRIMARY KEY, iteam TEXT, sold INTEGER, launched INTEGER, price INTEGER);
INSERT INTO makeup VALUES (1, "blush", 125, 2015, 19.25);
INSERT INTO makeup VALUES (2, "lipstick", 148, 2018, 8.99);
INSERT INTO makeup VALUES (3, "eyeshadow", 256, 2018, 15.85);
INSERT INTO makeup VALUES (4, "highlighter", 225, 2019, 8.99);
INSERT INTO makeup VALUES (5, "lip gloss", 256, 2020, 8.95);
INSERT INTO makeup VALUES (6, "eyeliner", 135, 2021, 11.99);
INSERT INTO makeup VALUES (7, "lip liner", 225, 2021, 11.99);
INSERT INTO makeup VALUES (8, "mascara", 365, 2020, 14.95);
INSERT INTO makeup VALUES (9, "foundation", 365, 2021, 24.99);
INSERT INTO makeup VALUES (10, "primer", 247, 2021, 11.99);
INSERT INTO makeup VALUES (11, "setting powder", 298, 2020, 13.99);
INSERT INTO makeup VALUES (12, "pressed powder", 183, 2021, 9.99);
INSERT INTO makeup VALUES (13, "bronzer", 136, 2020, 8.99);
INSERT INTO makeup VALUES (14, "lip balm", 122, 2021, 5.99);
INSERT INTO makeup VALUES (15, "moisterizer", 189, 2022, 12.88);
INSERT INTO makeup VALUES (16, "liquid eyeliner", 124, 2021, 12.99);
SELECT * FROM makeup ORDER BY price;
SELECT * FROM makeup ORDER BY launched;
SELECT * FROM makeup ORDER BY sold;
SELECT SUM(sold) FROM makeup;
