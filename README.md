#include<iostream>
#include <SFML/Graphics.hpp>
#include <SFML\Config.hpp>
#include<SFML/System.hpp>
#include<SFML/Window.hpp>
using namespace sf;
using namespace std;
int main()
{

    RenderWindow window(sf::VideoMode(850, 850), "chess board");
    Texture texturec8;
    texturec8.loadFromFile("bbishop.jpg");
    Texture texturef8;
    texturef8.loadFromFile("bbishoopb.jpg");
    Texture texturee8;
    texturee8.loadFromFile("bking.jpg");
    Texture textured8;
    textured8.loadFromFile("bqueen.jpg");
    Texture textured1;
    textured1.loadFromFile("wqueen.jpg");
    Texture texturee1;
    texturee1.loadFromFile("wking.jpg");
    Texture textureb8;
    textureb8.loadFromFile("bkinght.jpg");
    Texture textureg8;
    textureg8.loadFromFile("bknightw.jpg");
    Texture texturebpb;
    texturebpb.loadFromFile("bpawnb.jpg");
    Texture texturebpw;
    texturebpw.loadFromFile("bpawnw.jpg");
    Texture textureh8;
    textureh8.loadFromFile("brook.jpg");
    Texture texturea8;
    texturea8.loadFromFile("brook8.jpg");
    Texture texturea7;
    texturea7.loadFromFile("bpawn7.jpg");
    Texture texturea1;
    texturea1.loadFromFile("wrook1.jpg");
    Texture textureh1;
    textureh1.loadFromFile("wrookh.jpg");
    Texture textureg1;
    textureg1.loadFromFile("wknightb.jpg");
    Texture textureb1;
    textureb1.loadFromFile("wknightw.jpg");
    Texture texturef1;
    texturef1.loadFromFile("wbishopw.jpg");
    Texture texturec1;
    texturec1.loadFromFile("wbishopb.jpg");
    Texture texturewpw;
    texturewpw.loadFromFile("wpawnw.jpg");
    Texture texturewpb;
    texturewpb.loadFromFile("wpawnb.jpg");
    Texture texture1;
    texture1.loadFromFile("w.jpg");
    Texture texture;
    texture.loadFromFile("b.jpg");
    Texture texturea5;
    texturea5.loadFromFile("5.jpg");
    Texture texturea6;
    texturea6.loadFromFile("6.jpg");
    Texture texturea3;
    texturea3.loadFromFile("3.jpg");
    Texture texturea4;
    texturea4.loadFromFile("4.jpg");
    Texture texturea2;
    texturea2.loadFromFile("wpawn2.jpg");

    while (window.isOpen())
    {

        sf::Event event;
        while (window.pollEvent(event))
        {

            if (event.type == sf::Event::Closed)
                window.close();
        }



        Sprite sprite1;
        sprite1.setTexture(texturea8);
        sprite1.setPosition(sf::Vector2f(25.f, 25.f));
        sprite1.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite2;
        sprite2.setTexture(textureb8);
        sprite2.setPosition(sf::Vector2f(125.f, 25.f));
        sprite2.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite3;
        sprite3.setTexture(texturec8);
        sprite3.setPosition(sf::Vector2f(225.f, 25.f));
        sprite3.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite4;
        sprite4.setTexture(textured8);
        sprite4.setPosition(sf::Vector2f(325.f, 25.f));
        sprite4.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite5;
        sprite5.setTexture(texturee8);
        sprite5.setPosition(sf::Vector2f(425.f, 25.f));
        sprite5.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite6;
        sprite6.setTexture(texturef8);
        sprite6.setPosition(sf::Vector2f(525.f, 25.f));
        sprite6.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite7;
        sprite7.setTexture(textureg8);
        sprite7.setPosition(sf::Vector2f(625.f, 25.f));
        sprite7.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite8;
        sprite8.setTexture(textureh8);
        sprite8.setPosition(sf::Vector2f(725.f, 25.f));
        sprite8.setScale(sf::Vector2f(1.f, 1.f));

        Sprite spritel;
        spritel.setTexture(texture);
        spritel.setPosition(sf::Vector2f(0.f, 25.f));
        spritel.setScale(sf::Vector2f(.25f, 8.f));

        Sprite spriteup;
        spriteup.setTexture(texture);
        spriteup.setPosition(sf::Vector2f(0.f, 0.f));
        spriteup.setScale(sf::Vector2f(8.5f, 0.25f));

        Sprite spritedown;
        spritedown.setTexture(texture);
        spritedown.setPosition(sf::Vector2f(0.f, 825.f));
        spritedown.setScale(sf::Vector2f(8.5f, 0.25f));

        Sprite spriter;
        spriter.setTexture(texture);
        spriter.setPosition(sf::Vector2f(825.f, 25.f));
        spriter.setScale(sf::Vector2f(.25f, 8.f));

        Sprite sprite11;
        sprite11.setTexture(texturea7);
        sprite11.setPosition(sf::Vector2f(25.f, 125.f));
        sprite11.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite12;
        sprite12.setTexture(texturebpw);
        sprite12.setPosition(sf::Vector2f(125.f, 125.f));
        sprite12.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite13;
        sprite13.setTexture(texturebpb);
        sprite13.setPosition(sf::Vector2f(225.f, 125.f));
        sprite13.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite14;
        sprite14.setTexture(texturebpw);
        sprite14.setPosition(sf::Vector2f(325.f, 125.f));
        sprite14.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite15;
        sprite15.setTexture(texturebpb);
        sprite15.setPosition(sf::Vector2f(425.f, 125.f));
        sprite15.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite16;
        sprite16.setTexture(texturebpw);
        sprite16.setPosition(sf::Vector2f(525.f, 125.f));
        sprite16.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite17;
        sprite17.setTexture(texturebpb);
        sprite17.setPosition(sf::Vector2f(625.f, 125.f));
        sprite17.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite18;
        sprite18.setTexture(texturebpw);
        sprite18.setPosition(sf::Vector2f(725.f, 125.f));
        sprite18.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite21;
        sprite21.setTexture(texturea6);
        sprite21.setPosition(sf::Vector2f(25.f, 225.f));
        sprite21.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite22;
        sprite22.setTexture(texture);
        sprite22.setPosition(sf::Vector2f(125.f, 225.f));
        sprite22.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite23;
        sprite23.setTexture(texture1);
        sprite23.setPosition(sf::Vector2f(225.f, 225.f));
        sprite23.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite24;
        sprite24.setTexture(texture);
        sprite24.setPosition(sf::Vector2f(325.f, 225.f));
        sprite24.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite25;
        sprite25.setTexture(texture1);
        sprite25.setPosition(sf::Vector2f(425.f, 225.f));
        sprite25.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite26;
        sprite26.setTexture(texture);
        sprite26.setPosition(sf::Vector2f(525.f, 225.f));
        sprite26.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite27;
        sprite27.setTexture(texture1);
        sprite27.setPosition(sf::Vector2f(625.f, 225.f));
        sprite27.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite28;
        sprite28.setTexture(texture);
        sprite28.setPosition(sf::Vector2f(725.f, 225.f));
        sprite28.setScale(sf::Vector2f(1.f, 1.f));
        Sprite sprite31;
        sprite31.setTexture(texturea5);
        sprite31.setPosition(sf::Vector2f(25.f, 325.f));
        sprite31.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite32;
        sprite32.setTexture(texture1);
        sprite32.setPosition(sf::Vector2f(125.f, 325.f));
        sprite32.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite33;
        sprite33.setTexture(texture);
        sprite33.setPosition(sf::Vector2f(225.f, 325.f));
        sprite33.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite34;
        sprite34.setTexture(texture1);
        sprite34.setPosition(sf::Vector2f(325.f, 325.f));
        sprite34.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite35;
        sprite35.setTexture(texture);
        sprite35.setPosition(sf::Vector2f(425.f, 325.f));
        sprite35.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite36;
        sprite36.setTexture(texture1);
        sprite36.setPosition(sf::Vector2f(525.f, 325.f));
        sprite36.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite37;
        sprite37.setTexture(texture);
        sprite37.setPosition(sf::Vector2f(625.f, 325.f));
        sprite37.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite38;
        sprite38.setTexture(texture1);
        sprite38.setPosition(sf::Vector2f(725.f, 325.f));
        sprite38.setScale(sf::Vector2f(1.f, 1.f));
        Sprite sprite41;
        sprite41.setTexture(texturea4);
        sprite41.setPosition(sf::Vector2f(25.f, 425.f));
        sprite41.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite42;
        sprite42.setTexture(texture);
        sprite42.setPosition(sf::Vector2f(125.f, 425.f));
        sprite42.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite43;
        sprite43.setTexture(texture1);
        sprite43.setPosition(sf::Vector2f(225.f, 425.f));
        sprite43.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite44;
        sprite44.setTexture(texture);
        sprite44.setPosition(sf::Vector2f(325.f, 425.f));
        sprite44.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite45;
        sprite45.setTexture(texture1);
        sprite45.setPosition(sf::Vector2f(425.f, 425.f));
        sprite45.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite46;
        sprite46.setTexture(texture);
        sprite46.setPosition(sf::Vector2f(525.f, 425.f));
        sprite46.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite47;
        sprite47.setTexture(texture1);
        sprite47.setPosition(sf::Vector2f(625.f, 425.f));
        sprite47.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite48;
        sprite48.setTexture(texture);
        sprite48.setPosition(sf::Vector2f(725.f, 425.f));
        sprite48.setScale(sf::Vector2f(1.f, 1.f));
        Sprite sprite51;
        sprite51.setTexture(texturea3);
        sprite51.setPosition(sf::Vector2f(25.f, 525.f));
        sprite51.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite52;
        sprite52.setTexture(texture1);
        sprite52.setPosition(sf::Vector2f(125.f, 525.f));
        sprite52.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite53;
        sprite53.setTexture(texture);
        sprite53.setPosition(sf::Vector2f(225.f, 525.f));
        sprite53.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite54;
        sprite54.setTexture(texture1);
        sprite54.setPosition(sf::Vector2f(325.f, 525.f));
        sprite54.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite55;
        sprite55.setTexture(texture);
        sprite55.setPosition(sf::Vector2f(425.f, 525.f));
        sprite55.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite56;
        sprite56.setTexture(texture1);
        sprite56.setPosition(sf::Vector2f(525.f, 525.f));
        sprite56.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite57;
        sprite57.setTexture(texture);
        sprite57.setPosition(sf::Vector2f(625.f, 525.f));
        sprite57.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite58;
        sprite58.setTexture(texture1);
        sprite58.setPosition(sf::Vector2f(725.f, 525.f));
        sprite58.setScale(sf::Vector2f(1.f, 1.f));
        Sprite sprite61;
        sprite61.setTexture(texturea2);
        sprite61.setPosition(sf::Vector2f(25.f, 625.f));
        sprite61.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite62;
        sprite62.setTexture(texturewpb);
        sprite62.setPosition(sf::Vector2f(125.f, 625.f));
        sprite62.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite63;
        sprite63.setTexture(texturewpw);
        sprite63.setPosition(sf::Vector2f(225.f, 625.f));
        sprite63.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite64;
        sprite64.setTexture(texturewpb);
        sprite64.setPosition(sf::Vector2f(325.f, 625.f));
        sprite64.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite65;
        sprite65.setTexture(texturewpw);
        sprite65.setPosition(sf::Vector2f(425.f, 625.f));
        sprite65.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite66;
        sprite66.setTexture(texturewpb);
        sprite66.setPosition(sf::Vector2f(525.f, 625.f));
        sprite66.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite67;
        sprite67.setTexture(texturewpw);
        sprite67.setPosition(sf::Vector2f(625.f, 625.f));
        sprite67.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite68;
        sprite68.setTexture(texturewpb);
        sprite68.setPosition(sf::Vector2f(725.f, 625.f));
        sprite68.setScale(sf::Vector2f(1.f, 1.f));
        Sprite sprite71;
        sprite71.setTexture(texturea1);
        sprite71.setPosition(sf::Vector2f(25.f, 725.f));
        sprite71.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite72;
        sprite72.setTexture(textureb1);
        sprite72.setPosition(sf::Vector2f(125.f, 725.f));
        sprite72.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite73;
        sprite73.setTexture(texturec1);
        sprite73.setPosition(sf::Vector2f(225.f, 725.f));
        sprite73.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite74;
        sprite74.setTexture(textured1);
        sprite74.setPosition(sf::Vector2f(325.f, 725.f));
        sprite74.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite75;
        sprite75.setTexture(texturee1);
        sprite75.setPosition(sf::Vector2f(425.f, 725.f));
        sprite75.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite76;
        sprite76.setTexture(texturef1);
        sprite76.setPosition(sf::Vector2f(525.f, 725.f));
        sprite76.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite77;
        sprite77.setTexture(textureg1);
        sprite77.setPosition(sf::Vector2f(625.f, 725.f));
        sprite77.setScale(sf::Vector2f(1.f, 1.f));

        Sprite sprite78;
        sprite78.setTexture(textureh1);
        sprite78.setPosition(sf::Vector2f(725.f, 725.f));
        sprite78.setScale(sf::Vector2f(1.f, 1.f));


        window.clear(sf::Color::Black);
       
        window.draw(spriteup);
        window.draw(spritedown);
        window.draw(spriter);
        window.draw(spritel);
        window.draw(sprite1);
        window.draw(sprite2);
        window.draw(sprite3);
        window.draw(sprite4);
        window.draw(sprite5);
        window.draw(sprite6);
        window.draw(sprite7);
        window.draw(sprite8);
        window.draw(sprite11);
        window.draw(sprite12);
        window.draw(sprite13);
        window.draw(sprite14);
        window.draw(sprite15);
        window.draw(sprite16);
        window.draw(sprite17);
        window.draw(sprite18);
        window.draw(sprite21);
        window.draw(sprite22);
        window.draw(sprite23);
        window.draw(sprite24);
        window.draw(sprite25);
        window.draw(sprite26);
        window.draw(sprite27);
        window.draw(sprite28);
        window.draw(sprite31);
        window.draw(sprite32);
        window.draw(sprite33);
        window.draw(sprite34);
        window.draw(sprite35);
        window.draw(sprite36);
        window.draw(sprite37);
        window.draw(sprite38);
        window.draw(sprite41);
        window.draw(sprite42);
        window.draw(sprite43);
        window.draw(sprite44);
        window.draw(sprite45);
        window.draw(sprite46);
        window.draw(sprite47);
        window.draw(sprite48);
        window.draw(sprite51);
        window.draw(sprite52);
        window.draw(sprite53);
        window.draw(sprite54);
        window.draw(sprite55);
        window.draw(sprite56);
        window.draw(sprite57);
        window.draw(sprite58);
        window.draw(sprite61);
        window.draw(sprite62);
        window.draw(sprite63);
        window.draw(sprite64);
        window.draw(sprite65);
        window.draw(sprite66);
        window.draw(sprite67);
        window.draw(sprite68);
        window.draw(sprite71);
        window.draw(sprite72);
        window.draw(sprite73);
        window.draw(sprite74);
        window.draw(sprite75);
        window.draw(sprite76);
        window.draw(sprite77);
        window.draw(sprite78);

        window.display();
    }

    return 0;
}
