# Uncomment the next line to define a global platform for your project
platform :ios, '10.0'
source 'https://github.com/CocoaPods/Specs.git'

target '1v1Call-demo-swift' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  
  pod 'AgoraRtcEngine_iOS/RtcBasic'
  pod 'HyphenateChat'
  pod 'EaseCallKit'
  
  post_install do |installer|
    installer.generated_projects.each do |project|
      project.targets.each do |target|
          target.build_configurations.each do |config|
              config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '11.0'
           end
      end
    end
  end
  
end
