platform :ios, '12.0'
use_frameworks!

# workaround to avoid Xcode caching of Pods that requires
# Product -> Clean Build Folder after new Cordova plugins installed
# Requires CocoaPods 1.6 or newer
install! 'cocoapods', :disable_input_output_paths => true

def capacitor_pods
  pod 'Capacitor', :path => '../../../node_modules/@capacitor/ios'
  pod 'CapacitorCordova', :path => '../../../node_modules/@capacitor/ios'
  pod 'CapacitorCamera', :path => '../../node_modules/@capacitor/camera'
  pod 'CapacitorSplashScreen', :path => '../../node_modules/@capacitor/splash-screen'
end

target 'App' do
  capacitor_pods
  # Add your Pods here
end
