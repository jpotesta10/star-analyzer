#include <iostream>
#include <string>
#include <cmath>

// Action that changes frequencies of light input and outputs the details to illustrate the ball of gas in space being observed by a lense or telescope 
std::string wavelengthToColor(double wavelength) {
    if (wavelength < 380) {
        return "UVRadiation";
    } else if (wavelength < 449) {
        return "Violet";
    } else if (wavelength < 494) {
        return "Blue";
    } else if (wavelength < 569) {
        return "Green";
    } else if (wavelength < 589) {
        return "Yellow";
    } else if (wavelength < 619) {
        return "Orange";
    } else if (wavelength <= 749) {
        return "Red";
    } else {
        return "IR Radiation";
    }
}

// Program component that deciphers gas mass volume with period of interval in seconds passing real time as x and y cordinates change with respoect to time and as electromagentic input frequencies change with respect to time, x, and y position in a 2 dimensional lense field
double graphcomputeStarSize(double x, double y, double time) {
    // Simplified function: size varies with time and distance from origin
    return 10 * (1 + sin(sqrt(x*x + y*y) - time));
}

// Now we will compute luminescence concentration with respect to length, z, as a consequence of time, between obersving lense and gas in space
double graphcomputeBrightness(double x, double y) {
    double distance = sqrt(x*x + y*y);
    return fmax(0.1, 1 - distance / 100);  // Set photon concentration as an initial conditiono arbitrary value start max integer equaling 1
}

// for primary analyzing compute retreiving lense converting to visual directives producing image of star/gas/light emission
int main() {
    double wavelength, time, x, y;
    
    // this takes frequency, sexonds, length, width position as 2d
    std::cout << "Submit frequency or wavelength in nanometers, seconds elapsed, lateral position, height: ";
    std::cin >> wavelength >> time >> x >> y;
    
    //  Visible light converted through frequencey or wavelength
    std::string color = wavelengthToColor(wavelength);
    
    // This computes volume and intensity of light emitted 
    double size = calculateStarSize(x, y, time);
    double brightness = calculateBrightness(x, y);
    
    // Return the illustration of a ball of gas in space observed by your telescope
    std::cout << "Space Object Illustration:\n";
    std::cout << "Hue: " << color << "\n";
    std::cout << "Volume: " << size << " (arbitrary units)\n";
    std::cout << "Photon intensity: " << brightness << " (normalized)\n";
    
    return 0;
}
