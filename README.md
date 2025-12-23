# Date:23.12.2025

# Aim:
To design a user-friendly Event Registration Web Application using Figma that allows users to view event details and register for an event through an interactive and visually appealing user interface.
# Procedure:
1.	Figma was opened using a web browser and a new design file was created for the Event Registration Web Application.
2.	A web frame with standard desktop dimensions was selected to design the application layout.
3.	The Home Page was designed by adding the application title, navigation menu, event banner, and buttons such as View Events and Register Now.
4.	An Event Details Page was created to display information such as event name, date, time, venue, and event description.
5.	A Registration Form Page was designed with input fields for user details including Name, Email ID, Phone Number, and Event Name.
6.	Action buttons like Submit and Reset were added to the registration form for user interaction.
7.	A Confirmation Page was designed to display a successful registration message after form submission.
8.	Finally, the Figma project was saved and shared for demonstration and evaluation.

# Program
```
UI PAGE:
import { Button } from "./ui/button";
import { Card, CardContent } from "./ui/card";
import { Calendar, MapPin, User } from "lucide-react";

interface HomePageProps {
  onNavigate: (page: string) => void;
}

export function HomePage({ onNavigate }: HomePageProps) {
  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100">
      {/* Navigation */}
      <nav className="bg-white shadow-md">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="flex justify-between items-center h-16">
            <h1 className="text-indigo-600">Event Management System</h1>
            <div className="flex gap-6">
              <button
                onClick={() => onNavigate("home")}
                className="text-gray-700 hover:text-indigo-600 transition-colors"
              >
                Home
              </button>
              <button
                onClick={() => onNavigate("events")}
                className="text-gray-700 hover:text-indigo-600 transition-colors"
              >
                Events
              </button>
              <button
                onClick={() => onNavigate("register")}
                className="text-gray-700 hover:text-indigo-600 transition-colors"
              >
                Register
              </button>
            </div>
          </div>
        </div>
      </nav>

      {/* Hero Section */}
      <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
        <div className="text-center mb-12">
          <h2 className="text-indigo-600 mb-4">Welcome to CodeFest 2026</h2>
          <p className="text-gray-600 max-w-2xl mx-auto">
            Join us for an exciting coding competition and tech event at Saveetha Engineering College, Chennai
          </p>
        </div>

        {/* Event Banner */}
        <Card className="mb-12 overflow-hidden bg-gradient-to-r from-indigo-500 to-purple-600 text-white">
          <CardContent className="p-8">
            <div className="grid md:grid-cols-2 gap-8">
              <div>
                <h3 className="mb-4 text-white">CodeFest 2026</h3>
                <div className="space-y-3">
                  <div className="flex items-center gap-3">
                    <Calendar className="w-5 h-5" />
                    <span>January 11, 2026</span>
                  </div>
                  <div className="flex items-center gap-3">
                    <MapPin className="w-5 h-5" />
                    <span>Majestorium Hall, Saveetha Engineering College, Chennai</span>
                  </div>
                  <div className="flex items-center gap-3">
                    <User className="w-5 h-5" />
                    <span>Coordinator: Jeevanantham C</span>
                  </div>
                </div>
              </div>
              <div className="flex flex-col justify-center gap-4">
                <p className="text-white/90">
                  Experience a day filled with coding challenges, networking opportunities, and technical workshops. Don't miss this opportunity to showcase your skills!
                </p>
                <div className="flex gap-4">
                  <Button
                    onClick={() => onNavigate("events")}
                    variant="secondary"
                    size="lg"
                  >
                    View Events
                  </Button>
                  <Button
                    onClick={() => onNavigate("register")}
                    variant="outline"
                    size="lg"
                    className="bg-white text-indigo-600 hover:bg-gray-100"
                  >
                    Register Now
                  </Button>
                </div>
              </div>
            </div>
          </CardContent>
        </Card>

        {/* Features */}
        <div className="grid md:grid-cols-3 gap-6">
          <Card>
            <CardContent className="p-6">
              <div className="text-indigo-600 mb-3"></div>
              <h4 className="mb-2">Competitions</h4>
              <p className="text-gray-600">
                Participate in exciting coding competitions and win amazing prizes
              </p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-6">
              <div className="text-indigo-600 mb-3"></div>
              <h4 className="mb-2">Workshops</h4>
              <p className="text-gray-600">
                Learn from industry experts through hands-on technical workshops
              </p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-6">
              <div className="text-indigo-600 mb-3"></div>
              <h4 className="mb-2">Networking</h4>
              <p className="text-gray-600">
                Connect with fellow developers and build lasting professional relationships
              </p>
            </CardContent>
          </Card>
        </div>
      </div>
    </div>
  );
}

```

# Output:
<img width="1905" height="859" alt="Screenshot 2025-12-23 085854" src="https://github.com/user-attachments/assets/ee15144a-285d-489e-b99a-91f6d5edae68" />
<img width="1900" height="847" alt="Screenshot 2025-12-23 085921" src="https://github.com/user-attachments/assets/782c7ed1-a679-4a3e-aca5-084cbde4efbb" />
<img width="1894" height="823" alt="Screenshot 2025-12-23 090033" src="https://github.com/user-attachments/assets/12df2ecc-b93c-4da2-af9d-6c8474df29cc" />
<img width="1896" height="847" alt="Screenshot 2025-12-23 090224" src="https://github.com/user-attachments/assets/e89dde59-b916-4b5e-99de-e7cac6d1c02e" />


# Result
Thus, an Event Registration Web Application was successfully designed using Figma. The design includes multiple interactive screens such as the home page, event details page, registration form, and confirmation page.
