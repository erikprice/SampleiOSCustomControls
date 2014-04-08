platform :ios, '6.1'

pod 'Brightcove-Player-SDK'
pod 'Brightcove-Player-SDK-IMA'

# Remove 64-bit build architecture from Pods targets
post_install do |installer|
  installer.project.targets.each do |target|
      target.build_configurations.each do |configuration|
            target.build_settings(configuration.name)['ARCHS'] = '$(ARCHS_STANDARD_32_BIT)'
      end
  end
end

