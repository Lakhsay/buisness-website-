import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

const BusinessWebsite = () => {
  return (
    <div className="min-h-screen bg-gray-100">
      {/* Header Section */}
      <header className="bg-blue-600 text-white py-4">
        <div className="container mx-auto flex justify-between items-center">
          <h1 className="text-2xl font-bold">Your Business Name</h1>
          <nav className="space-x-4">
            <a href="#services" className="hover:underline">Services</a>
            <a href="#about" className="hover:underline">About</a>
            <a href="#contact" className="hover:underline">Contact</a>
          </nav>
        </div>
      </header>

      {/* Hero Section */}
      <section className="bg-white py-16">
        <div className="container mx-auto text-center">
          <h2 className="text-4xl font-bold mb-4">Welcome to Our Business</h2>
          <p className="text-lg text-gray-600 mb-6">We provide top-notch services to help your business grow.</p>
          <Button className="bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 text-lg rounded-full">
            Get Started
          </Button>
        </div>
      </section>

      {/* Services Section */}
      <section id="services" className="py-16 bg-gray-100">
        <div className="container mx-auto text-center">
          <h3 className="text-3xl font-bold mb-6">Our Services</h3>
          <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
            <Card className="shadow-lg">
              <CardContent>
                <h4 className="text-xl font-bold mb-2">Service 1</h4>
                <p className="text-gray-600">Description of the first service offered.</p>
              </CardContent>
            </Card>
            <Card className="shadow-lg">
              <CardContent>
                <h4 className="text-xl font-bold mb-2">Service 2</h4>
                <p className="text-gray-600">Description of the second service offered.</p>
              </CardContent>
            </Card>
            <Card className="shadow-lg">
              <CardContent>
                <h4 className="text-xl font-bold mb-2">Service 3</h4>
                <p className="text-gray-600">Description of the third service offered.</p>
              </CardContent>
            </Card>
          </div>
        </div>
      </section>

      {/* About Section */}
      <section id="about" className="py-16 bg-white">
        <div className="container mx-auto text-center">
          <h3 className="text-3xl font-bold mb-6">About Us</h3>
          <p className="text-gray-600">We are a passionate team dedicated to delivering exceptional results for our clients. Our mission is to provide solutions that drive success.</p>
        </div>
      </section>

      {/* Contact Section */}
      <section id="contact" className="py-16 bg-gray-100">
        <div className="container mx-auto text-center">
          <h3 className="text-3xl font-bold mb-6">Contact Us</h3>
          <p className="text-gray-600 mb-4">Have questions? We’d love to hear from you!</p>
          <Button className="bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 text-lg rounded-full">
            Get in Touch
          </Button>
        </div>
      </section>

      {/* Footer Section */}
      <footer className="bg-blue-600 text-white py-4">
        <div className="container mx-auto text-center">
          <p>&copy; {new Date().getFullYear()} Your Business Name. All rights reserved.</p>
        </div>
      </footer>
    </div>
  );
};

export default BusinessWebsite;
