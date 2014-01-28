Echelon::Application.routes.draw do

  root :to => 'home#index'
  match 'contact-us' => 'home#contact_us'
  match 'get-started' => 'home#get_started'
  match 'iiot-at-work' => 'home#iiot_at_work'
  match 'izot-platform' => 'home#izot_platform'
  match 'support' => 'home#support'
  match 'iiot-at-work/stories/:id' => 'home#stories'
  match 'industry-perspective' => 'home#industry_perspective'
  match 'white-paper' =>'home#whitepaper'
  match 'download' => 'home#get_started'
  match 'executive-summary' => 'home#executive_summary'
  match 'lonworks' => 'home#lonworks'
  match 'izot-presentation' => 'home#izot_presentation'
  

  resources :izot_products, :path => 'izot-products' do
    collection do
      get 'modules'
      get 'chips'
      get 'device_stacks', :path => 'device-stacks'
      get 'network_interfaces', :path => 'network-interfaces'
      get 'commissioning_tool', :path => 'commissioning-tool'
      get 'network_services_server', :path => 'network-services-server'
      get 'router_and_network_interface_software', :path => 'router-and-network-interface-software'
      get 'routers'
    end
  end
end
