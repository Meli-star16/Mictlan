import flet as ft


def main(page: ft.page):
#Establece tamaño de pantalla

    page.window_width=800
    page.window_width=800
    
    page.bgcolor="black"
    page.title="Mictlan"
    page.fgcolor="gray"
    
    Intro=ft.Audio(scr="Intro.mp3", volume=1, balance=0)
    page.overlay.append(Intro)
    
    PrimerNivel=ft.Audio(scr="Primer_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(PrimerNivel)
    
    SegundoNivel=ft.Audio(scr="Segundo_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(SegundoNivel)
    
    TercerNivel=ft.Audio(scr="Tercer_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(TercerNivel)
    
    CuartoNivel=ft.Audio(scr="Cuarto_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(CuartoNivel)
    
    QuintoNivel=ft.Audio(scr="Quinto_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(QuintoNivel)
    
    SextoNivel=ft.Audio(scr="Sexto_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(SextoNivel)
    
    SeptimoNivel=ft.Audio(scr="Septimo_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(SeptimoNivel)
    
    OctavoNivel=ft.Audio(scr="Octavo_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(OctavoNivel)
    
    NovenoNivel=ft.Audio(scr="Noveno_Nivel.mp3", volume=1, balance=0)
    page.overlay.append(NovenoNivel)
    
#Crear la interfaz
    btnIntro=ft.FilledButton(text="Escuchar el intro", disabled=False)
    
    btnNivel1=ft.ElevatedButton(text="Primer Nivel")
    img1=ft.Image(src="Primer-Nivel.jpeg", width=150, heigth=150)
    
    btnNivel2=ft.ElevatedButton(text="Segundo Nivel")
    img2=ft.Image(src="Segundo-Nivel.jpeg", width=150, heigth=150)
    
    btnNivel3=ft.ElevatedButton(text="Tercer Nivel")
    img3=ft.Image(src="Tercer-Nivel.png", width=150, heigth=150)
    
    btnNivel4=ft.ElevatedButton(text="Cuarto Nivel")
    img4=ft.Image(src="Cuarto-Nivel.jpeg", width=150, heigth=150)
    
    btnNivel5=ft.ElevatedButton(text="Quinto Nivel")
    img5=ft.Image(src="Quinto-Nivel.jpeg", width=150, heigth=150)
    
    btnNivel6=ft.ElevatedButton(text="Sexto Nivel")
    img6=ft.Image(src="Sexto-Nivel.jpeg", width=150, heigth=150)
    
    btnNivel7=ft.ElevatedButton(text="Septimo Nivel")
    img7=ft.Image(src="Septimo-Nivel.peg", width=150, heigth=150)
    
    btnNivel8=ft.ElevatedButton(text="Octavo Nivel")
    img8=ft.Image(src="Octavo-Nivel.png", width=150, heigth=150)
    
    btnNivel9=ft.ElevatedButton(text="Noveno Nivel")
    img9=ft.Image(src="Noveno-Nivel.jpeg", width=150, heigth=150)
    
    
    page.add(
            ft.Row(
                alignment="star",
                controls=[btnIntro]
            ),
            ft.Column(
                alignment="CENTER",
                apacing=10,
                acroll=ft.ScrollMode.Auto,
                controls=[
                    ft.Row(
                        alignment="CENTER",
                        controls=[btnNivel1, img1]
                    ),
                    ft.Column(
                        alignment="CENTER",
                        controls=[btnNivel2, img2]
                    ),
                    ft.Column(
                        alignment="CENTER"
                        controls=[btnNivel3, img3]
                        ),
                ]
            )
            )
