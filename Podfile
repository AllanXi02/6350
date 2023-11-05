platform :ios, '9.0' 

target 'StockApp' do
  use_frameworks!

  pod 'RealmSwift'
  pod "Alamofire"
  pod "SwiftSpinner"
  pod 'SwiftyJSON'
end

post_install do |installer|
    installer.generated_projects.each do |project|
        project.targets.each do |target|
            target.build_configurations.each do |config|
                config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
            end
        end
    end
end