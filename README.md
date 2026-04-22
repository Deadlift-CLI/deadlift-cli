__| |_________________________________________________| |__
__   _________________________________________________   __
  | |                                                 | |  
  | | ____  _____    _    ____  _     ___ _____ _____ | |  
  | ||  _ \| ____|  / \  |  _ \| |   |_ _|  ___|_   _|| |  
  | || | | |  _|   / _ \ | | | | |    | || |_    | |  | |  
  | || |_| | |___ / ___ \| |_| | |___ | ||  _|   | |  | |  
  | ||____/|_____/_/   \_\____/|_____|___|_|     |_|  | |  
__| |_________________________________________________| |__
__   _________________________________________________   __
  | |                                                 | |  
=========================================================
                      ITC2205 B
             S/W Engineering Practices
          Instructor: Dr. Evgenia Vagianou
                    Spring 2026
                 Gym Booking System
           The American College of Greece
=========================================================



 ██████╗██████╗ ███████╗ █████╗ ████████╗███████╗██████╗     ██████╗ ██╗   ██╗
██╔════╝██╔══██╗██╔════╝██╔══██╗╚══██╔══╝██╔════╝██╔══██╗    ██╔══██╗╚██╗ ██╔╝
██║     ██████╔╝█████╗  ███████║   ██║   █████╗  ██║  ██║    ██████╔╝ ╚████╔╝ 
██║     ██╔══██╗██╔══╝  ██╔══██║   ██║   ██╔══╝  ██║  ██║    ██╔══██╗  ╚██╔╝  
╚██████╗██║  ██║███████╗██║  ██║   ██║   ███████╗██████╔╝    ██████╔╝   ██║   
 ╚═════╝╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝   ╚═╝   ╚══════╝╚═════╝     ╚═════╝    ╚═╝   

      Apostolos Kakarantzas | Erina Hoxha | Angelos Markopoulos






 ____ ____ ____ ____ ____ 
||A |||B |||O |||U |||T ||
||__|||__|||__|||__|||__||
|/__\|/__\|/__\|/__\|/__\|

Deadlift is a console-based gym booking system written in Python.
It allows members to browse, book, cancel and reschedule training
sessions (e.g. Pilates, Yoga, CrossFit), while giving admins full
control over sessions and user accounts.


 ____ ____ ____ _________ ____ ____ _________ ____ ____ ____ 
||H |||O |||W |||       |||T |||O |||       |||R |||U |||N ||
||__|||__|||__|||_______|||__|||__|||_______|||__|||__|||__||
|/__\|/__\|/__\|/_______\|/__\|/__\|/_______\|/__\|/__\|/__\|

Requirements: Python 3.8 or higher, no extra libraries needed.

  python main.py
 ____ ____ ____ ____ ____ ____ ____ ____ 
||A |||C |||C |||O |||U |||N |||T |||S ||
||__|||__|||__|||__|||__|||__|||__|||__||
|/__\|/__\|/__\|/__\|/__\|/__\|/__\|/__\|

  Username          Password    Role
  --------          --------    ----
  admin             admin123    Administrator
  john_d            pass123     User
  e_hoxha           pass123     User
  e_vagianou        pass123     User
  a_markopoulos     pass123     User

  No account? Select "Continue as Guest" to browse sessions without logging in.

  Forgot your password? Select "Forgot Password" from the main menu,
  enter your email, and a 6-digit reset token will be printed to the
  console. Enter the token and your new password to regain access.

Data is saved automatically to gym_data.json after every action.


 ____ ____ ____ ____ ____ ____ ____ ____ 
||O |||V |||E |||R |||V |||I |||E |||W ||
||__|||__|||__|||__|||__|||__|||__|||__||
|/__\|/__\|/__\|/__\|/__\|/__\|/__\|/__\|

  main.py       Entry point, all menus and navigation
  models.py     Core data classes (User, Session, Booking)
  database.py   Data storage and JSON persistence
  auth.py       Login and authentication
  display.py    Session listing, filters and terminal colours
  booking.py    Book, cancel and reschedule logic
  admin.py      Admin tools for managing sessions and users










   ▄▄▄▄▀ ▄  █ ██      ▄   █  █▀  ▄▄▄▄▄  
▀▀▀ █   █   █ █ █      █  █▄█   █     ▀▄
    █   ██▀▀█ █▄▄█ ██   █ █▀▄ ▄  ▀▀▀▀▄  
   █    █   █ █  █ █ █  █ █  █ ▀▄▄▄▄▀   
  ▀        █     █ █  █ █   █           
          ▀     █  █   ██  ▀            
               ▀                        
▄████  ████▄ █▄▄▄▄                      
█▀   ▀ █   █ █  ▄▀                      
█▀▀    █   █ █▀▀▌                       
█      ▀████ █  █                       
 █             █                        
  ▀           ▀                         
                                        
█▄▄▄▄ ▄███▄   ██   ██▄   ▄█    ▄     ▄▀ 
█  ▄▀ █▀   ▀  █ █  █  █  ██     █  ▄▀   
█▀▀▌  ██▄▄    █▄▄█ █   █ ██ ██   █ █ ▀▄ 
█  █  █▄   ▄▀ █  █ █  █  ▐█ █ █  █ █   █
  █   ▀███▀      █ ███▀   ▐ █  █ █  ███ 
 ▀              █           █   ██      
               ▀                        
